<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css/todolistcss.css">
    <style>
        *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: black;
}
.list{
    position: relative;
    background: #fff;
    width: 350px;
}
.list h2{
    background:skyblue;
    color: white;
    padding: 15px 0;
    font-weight: 600;
    text-align: center;
}
.list ul{
    position: relative;
    padding: 20px;
}
.list ul li{
    position: relative;
    list-style: none;
    padding: 15px 0;
    border-bottom:1px solid rgb(0,0,0,0.2);
}
.list ul li:last-child{
    border-bottom:none;
}
.list ul li label{
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
}
.list ul li label input{
    visibility: hidden;
    appearance: none;
}
.list ul li label p{
    position: absolute;
}
.list ul li label span{
    position: relative;
    width: 20px;
    height: 20px;
    border:1px solid #ccc;
    border-radius:50%;
}
.list ul li label span:before{
    content:'';
    position: absolute;
    top:5px;
    width: 10px;
    height: 5px;
    border-left:4px solid rgb(228, 218, 218);
    border-bottom: 2px solid rgb(228, 218, 218);
    transform: rotate(-45deg);
}
.list ul li label input:checked ~ p {
    text-decoration: line-through;
    color:rgb(161, 109, 109);
}
.list ul li label input:checked ~ span{
    background-color: #03a9f4;
    border:1px solid #03a9f4;
}
.list ul li label input:cheked ~ span:: before{
    border-left:2px solid #fff;
    border-bottom:2px solid #fff;
}
    </style>
</head>
<body>
    <div class="list">
        <h2>To Do List</h2>
        <ul>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Breakfast</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Lectures At 10am</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Household Work</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>college Work</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Meeting With Team</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Recruitment</p>
                    <span></span>
                </label>
            </li>
            <li>
                <label>
                    <input type="checkbox">
                    <p>Phone Call With Head</p>
                    <span></span>
                </label>
            </li>
        </ul>
    </div>
</body>
</html>
