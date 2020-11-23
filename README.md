<!DOCTYPE html>
<html>
    <head>
        <title>กรอกใบคำร้อง</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
        <link rel="preconnect" href="https://fonts.gstatic.com">
        <link href="https://fonts.googleapis.com/css2?family=Mitr:wght@600&display=swap" rel="stylesheet">
        <link rel="preconnect" href="https://fonts.gstatic.com">
        <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;500&display=swap" rel="stylesheet">  
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
        <script src="https://kit.fontawesome.com/a076d05399.js"></script>
        <!-- Latest compiled and minified CSS -->
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
        <!-- jQuery library -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
        <!-- Popper JS -->
        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
        <!-- Latest compiled JavaScript -->
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
        <style>
    .header {
        background-color: #eea15d;
        padding: 20px;
        text-align: center;
    }
    h1 {
        font-size: 70px;
        font-style: normal;
        font-family: "Mitr";
        
    }
    h2{
        font-size: 30px;
        font-style: normal;
        font-family: "Kanit";
        
    }   
    .center_type{
        background-color:  #f1f1f1;
    }
    .sideLeft{
        background-color:  #042f5a;
        width:220px;
        height:55px;
        font-size:15px;
        display:block;
        text-align:center;
        border:none;
        border-radius:2px;
        cursor:pointer;
        color: white;
    }
    .button{
        background-color:  #042f5a;
        
    }
    .button-wrapper{
        width:220px;
        height:55px;
        font-size:16px;
        display:block;
        /*text-align:center;*/
        border:none;
        border-radius:2px;
        cursor:pointer;
        color: white;
    }
    .posOfData{
        margin-top: -20px;
        margin-left: 300px;
    }
    .pos{
        margin-top: 5px;
    }
    .button1{
        padding: 15px 15px; 
        border-radius: 7px;
    
    }
    .Sarabun {
        font-family:  Sarabun;
    }
    .disabled {
        opacity: 0.6;
        cursor: not-allowed;
    }
    .aside {
        float: left;
        margin-top: 170px;
        border: 2px solid black;
        background-color: #f0a985;
        position: absolute;
        width:250px;
        height: 550px;
        align: center;
    }
    .area{
        padding: 10px;
        border: 1px solid #4CAF50;
        border-radius: 8px;
        background-color: rgb(182, 140, 85);
    }
    .bg-color {
        background-color: rgb(241, 237, 214);
        padding-bottom:100px;

    }
    .bg-color-content{
        background-color: #94705e;
       
    }
    table, tr,th {
        border: 2px solid black;
        padding: 5px;
    }
    .table {
        border-spacing: 10px;
    }
    footer{
        text-align: center;
        height: 50px;
        font-size: 20px;
        background-color: rgb(48, 46, 46);
        color: white; 
        
    }
    .right_box_area{
        
        border: 1px solid #f5fdf5;
        border-radius: 4px;
        background-color: rgb(245, 250, 242);
    }
    .box_right{
        width:220px;
        height:55px;
        border: 1px solid #4CAF50;
        border-radius: 5px;
        background-color: rgb(119, 177, 81);
        font-size: 15px;
        color: white;
        text-align: center;
    }
    </style>
    </head>
    <body>
        <div class="container-fluid header-height" >
            <h1 class= "header">ระบบการจดทะเบียนล่าช้า</h1>
<!--ส่วนซ้าย-->    
            <div class="container-fluid bg-color">
                <div class="row">
                  <div class="col-2 bg-color-content">
            
                        <button class="btn btn-primary button button1 button-wrapper pos" class="Sarabun" style="color:white">หน้าแรก</button><br>
                        <form action = "/fill-up/">
                        <button class="btn btn-primary button button1 button-wrapper " class="Sarabun" style="color:white ">กรอกคำร้องจดทะเบียนล่าช้า</button><br>
                        </form>
                        <button class="btn btn-primary button button1 button-wrapper disabled " class="Sarabun" style="color:white ">ตรวจสอบสถานะคำร้อง</button><br>
                        <button class="btn btn-primary button button1 button-wrapper disabled " class="Sarabun" style="color:white ">แสดงผลยื่นคำร้อง</button><br>
                        <button class="btn btn-primary button button1 button-wrapper disabled " class="Sarabun " style="color:white ">ชำระค่าลงทะเบียน</button><br>
                        <form action = "/logout/">
                        <button class="btn btn-primary button button1 button-wrapper" class="Sarabun" style="color:white ">ออกจากระบบ</button>
                        </form>
                       
                  </div>
<!--ส่วนตรงกลาง-->
<div class="col-8 " style="background-color: rgb(253, 252, 246); ">
    <h2>กรอกคำร้องจดทะเบียนล่าช้า</h2>
    <br>
    <h3 align="center" style="font-size:20px"> </h3>
        <form align="left">
            <div class="area" style="font-size: 16px;">
                <div style="background-color: cornsilk;">
                <table style="width: 100%;">
                  <tr>
                      <th ><label style="font-family:Kanit;" for ="term">ภาคเรียนที่ &nbsp; </label>
                        <select name="te" id="term01">
                          <option style="font-family:Kanit;" value="เทอมที่1">1/2563</option>
                          <option style="font-family:Kanit;" value="เทอมที่2">2/2563</option>
                          <option style="font-family:Kanit;" value="เทอมที่2">1/2564</option>
                          <option style="font-family:Kanit;" value="เทอมที่2">2/2564</option>
                          <select>
                              <div>
                                  <label style="font-family:Kanit;" for="idsubject">รหัสวิชา  &nbsp;&nbsp; &nbsp; &nbsp; </label>
                                  <input type="text" name="idsubject" id="idsubject" required>
                              </div>
                              <div>
                                  <label style="font-family:Kanit;" for="subjectname">ชื่อวิชา  &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; </label>
                                  <input  type="text" name="subjectname" id ="subjectname" required>
                              </div>
                              <div>
                                  <label style="font-family:Kanit;" for="sec">Sections    &nbsp; &nbsp; </label>
                                  <select name="te" id="sec01">
                                      <option value="650001">650001</option>
                                      <option value="650002">650002</option>
                                      <option value="650003">650003</option>
                                  </select>
                      </th>
                    <div>            
                      <th  style="width:58%">
                          <label style="font-family:Kanit;" for="comment">เหตุผลที่ยื่นคำร้อง:</label>
                             <textarea class="form-control" rows="5" style="font-size: 12px;" id="comment01" name="text"></textarea>
                      </th>
                        </select> 
                  </tr>
                </table>
              <br> 
                        <div ALIGN = "RIGHT" >                
                          <button type="button" class="btn btn-outline-secondary" onclick="register(1)" style="font-size: 14px; height:30px; border-radius: 3px; background-color:rgb(60, 168, 46); color: rgb(26, 25, 25);">ลงทะเบียน</button>
                          <input type="button" onclick="myFunction()" value="Reset form">
                        </div>
                        <br>
                    </div>
                    <script>
                      /*ฟังชั่นเพื่อให้มันรับค่าละก็เเสดงค่าเรื่อยๆ-->*/
                      let num = 0;
                      function register(next) {
                          num += next;
                          let table = document.getElementById("table");
                          let row = table.insertRow(-1); 
                          
              
                          for (let i = 0; i < 6; i++) {
                              cell = row.insertCell(i);
                              if (i == 0) {
                                  tnode = document.createTextNode(num);
                              }
                              if (i == 1) {
                                  tnode = document.createTextNode(document.getElementById("term01").value);
                              }
                              if (i == 2) {
                                  tnode = document.createTextNode(document.getElementById("idsubject").value);
                              }
                              if (i == 3) {
                                  tnode = document.createTextNode(document.getElementById("subjectname").value);
                              }
                              if (i == 4){
                                  tnode = document.createTextNode(document.getElementById("sec01").value)
                              }
                              if (i == 5){
                                  tnode = document.createTextNode(document.getElementById("comment01").value)
                              }
                              cell.appendChild(tnode);
                          }
                      }
                  </script>
                </div>
          
                <br>
                <table class="table" id="table">
                  <thead class="thead-dark">
                    <tr> <!--หัวตาราง-->
                      <th scope="col">ลำดับที่</th>
                      <th scope="col">เทอม</th>
                      <th scope="col">รหัสวิชา</th>
                      <th scope="col">ชื่อวิชา</th>
                      <th scope="col">Section</th>
                      <th scope="col">เหตุผลที่ยื่นคำร้อง</th>
                    </tr>
                  </thead>
                </table>
                <script>
                  function myFunction() {
                      document.getElementById("myForm").reset();
                  }
              </script>
    </form>
    <div ALIGN = "RIGHT">
        <br>
            <button type="submit" class="btn btn-primary" style="font-size: 16px;">Submit</button>     
        </div>
          
     <br>
    <hr>       
    <!--comment ด่านล่าง-->
    <div >
            <form>
                <div class="form-group" style="font-size:16px">
                  <label for="comment">Comment:</label>
                  <textarea class="form-control" rows="5" style="font-size:16px；" id="comment" name="text"></textarea>
                </div>
                <button type="submit" class="btn btn-primary" style="font-size:14px">Submit</button>
            </form>
    </div> 
    <br>
    <br>   
 </div>
                          
<!--ส่วนขวา-->

                  <div class="col-2 bg-color-content"> 
        
                      <div class="right_box_area">
                        <p><a class="box_right " href="https://reg.tu.ac.th/th/Picture/AttFile/c58f489e-8496-4565-845a-6eb97f6acbb6">ข้อกำหนดในการจดทะเบียนล่าช้า.pdf.</a></p>
                        <br>
                        <p><a class="box_right" href="https://drive.google.com/file/d/0B94Sg9FVXVtJVzRRZVBVaFF5bGs/view">รูปเเบบการเขียน.pdf.</a></p>  
                       </div>    
                  </div>
                </div>
              </div>
            
              <!-- footer -->
      <footer>
        <div >
            <p >TEL: 081-xxx-xxxx</p>
        </div>
    </footer>       
            </div>
    </body>
</html>
