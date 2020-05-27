```
<!DOCTYPE html>
<html>
    <head>
        <title>Login Form</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <form>
            <h2>Login Form</h2>
            <img src="256-512.webp">
        <div class="input-container">
            <img src="girl-128.webp">
             <input class="input-field" type="text"placeholder="User Name">
        </div>
        <div class="input-container">
            <img src="images.png">
            <input class="input-field" type="text" placeholder="Email">
        </div>
        <div class="input-container">
            <img src="download.png">
    <input class="input-field" type="password" placeholder="******">
    </div>
  </label><input type="checkbox" checked="checked" name="remember me">Remember Me</label><br>
    <button type="submit" class="btn">Login</button>
     </form>
    </body>
</html>
```
```
html , body {

    background:mediumturquoise;

 }

 form {
     background-color:mediumpurple;
     text-align:center;
     padding:10px 10px 10px 10px;
     width:350px;
     margin:auto;
     border-radius: 20px;
 }
    
    h2 {
    color:maroon;
    font-family: Arial, Helvetica, sans-serif;
    }
    
 form img{
     width:60px;
     height:60px;
     margin-top:20px;
     margin-bottom:20px;
     
 }
 .input-container {
    display:flex;
    margin-bottom:15px;
    height: 40px;
    justify-content:center;
    align-items: center;
    
 }
 .input-container img {
     width:30px;
     height: 30px;
     color:#fff;                                                                                                                                                                                                                                                                                                      
     justify-content:center;
     align-content: center;
     margin-right: 10px;
     border-radius: 20px;
    
 }
 .input-field {
     padding:5px 10px;
     border: 0;
     border-radius:20px;
     font-size:15px;
 }

 .btn {
     background-color:green;
     padding:10px 10px;
     border-radius:10px ;
     cursor:pointer;
     font-size:15px;
     margin:20px;
 }
 .btn:hover{
     background:orange;
     cursor: pointer;
 }
```
