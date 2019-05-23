---
title: 'Nguyễn Văn Chương'
media_order: 'con_address.png,con_tel.png,nguyen-van-chuong-2010.jpg'
---

#  Nguyễn Văn Chương
 
 ![Nguyễn Văn Chương](nguyen-van-chuong-2010.jpg)<br>
![address](con_address.png)
26 Lê Quang Sung, Thanh Khê<br>
Đà Nẵng<br>
Việt Nam<br>
![Số Điện Thoại :](con_tel.png) +84 2363712992<br>
[greensystem.vn](http://www.greensystem.vn)<br><br>

<form id="test-form" action="https://script.google.com/macros/s/AKfycbzaNoaa2sfFvX3oDiK736EomoRQailVAppaqMCE5oTJZ5Paf0M/exec" method="GET" name="gữi email"><br>
Nhập Tên&ensp;&ensp;: <input type="text" name="name" > <br>
Nhập Email : <input type="email" name="email" required><br>
<textarea rows="5" cols="40" name="description" placeholder="Ý kiến....">
</textarea> &ensp;&ensp;
    <button type="submit"id="submit-form">Gửi góp ý</button><br><br>
 </form>
 
 
<script src="http://code.jquery.com/jquery-1.12.0.min.js"></script>
<script type="text/javascript">
 $(document).ready(function()
 {   
   var submit = $("button[type='submit']");
   submit.click(function()
               {
                  var data = $('form#test-form').serialize();
                  $.ajax({
                            type : 'GET', 
                            url : 'https://script.google.com/macros/s/AKfycbzaNoaa2sfFvX3oDiK736EomoRQailVAppaqMCE5oTJZ5Paf0M/exec',
                            dataType:'json',
                            crossDomain : true,
                            data : data,
                            success : function(data)
                          { 
                  if(data == 'false') 
                          {
                             alert('Thêm không thành công');
                          }else{
                             alert('Đã thêm dữ liệu vào Form');
                              location.reload();
                          }
               }
    });
    return false;
   });
 });
</script>
