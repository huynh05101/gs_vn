---
title: 'Chuong NGUYEN'
media_order: 'con_address.png,con_tel.png,nguyen-van-chuong-2010.jpg'
---

# Chuong NGUYEN
 
 ![VanChuongNguyen](nguyen-van-chuong-2010.jpg)<br>
![address](con_address.png)
26 Le Quang Sung, Thanh Khe<br>
Da Nang<br>
Viet Nam<br>
![phone](con_tel.png) +84 2363712992<br>
[greensystem.vn](http://www.greensystem.vn)<br><br>

<form id="test-form" action="https://script.google.com/macros/s/AKfycbzaNoaa2sfFvX3oDiK736EomoRQailVAppaqMCE5oTJZ5Paf0M/exec" method="GET" name="gữi email"><br>
Enter your Name: <input type="text" name="name" > <br>
Enter your Email : <input type="email" name="email" required><br>
<textarea rows="5" cols="40" name="description" placeholder="Comment....">
</textarea> &ensp;&ensp;
    <button type="submit"id="submit-form"> Envoyer </button><br><br>
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
                             alert('KO');
                          }else{
                              alert(' added to the form ');
                              location.reload();
                          }
               }
    });
    return false;
   });
 });
</script>
