# Lab6Web  
### Nur Laila (312310149)  
### TI.23.A1  

## jQuery Effects – Sliding
```sh
<!DOCTYPE html>
<html 
<head>
    <script src=""http:ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
    </script>
    <script>
    $(document).ready(function(){
        $("#flip").click(function(){
            $("#panel").slideToggle("slow");
        });
    });
    </script>

    <style type="text/css">
        #panel, #flip {
            padding: 5px;
            text-align: center;
            background-color: #e5eecc;
            border: solid 1px #c3c3c3;
        }
        #panel {
            padding: 50px;
            display: none;
        }

    </style>
</head>
<body>
    <div id = "flip">Click to slide the panel down or up</div>
    <div id = "panel">Hello world!</div>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/a186cd70-3672-4e66-8b42-6c81dc0c4d6d)  
Kode ini membuat efek slide menggunakan jQuery. Saat `flip` diklik, `panel` akan muncul atau hilang dengan animasi slide.    

## jQuery Animation   
```sh
<!DOCTYPE html>
<html>
<head>
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
    </script>
    <script>
    $(document).ready(function(){
        $("button").click(function(){
            var div=$("div");
            div.animate({height:'300px',opacity:'0.4'}, "slow");
            div.animate({height:'300px',opacity:'0.8'}, "slow");
            div.animate({height:'100px',opacity:'0.4'}, "slow");
            div.animate({height:'100px',opacity:'0.8'}, "slow");
        });
    });
    </script>
</head>
<body>
    <button>Start Animation</button>
    <div style="background:#98bf21;height:100px;width:100px;position:absolute;"></div>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/07bd1112-04f7-4018-b327-6d27d6b55a34)    
![image](https://github.com/user-attachments/assets/6bb3f93e-1801-42d1-aee3-1aebfbe95cef)   
Kode ini menggunakan jQuery untuk membuat animasi pada elemen `<div>` saat tombol ditekan. Animasi mengubah tinggi dan opasitas `<div>` secara bertahap, bergerak antara tinggi 300px dan 100px dengan opasitas 0.4 dan 0.8, masing-masing dalam gerakan lambat.   

## jquery UI draggable  
```sh
<!DOCTYPE html>
<html>
<head>
    <title>Elemen yang Dapat Ditarik</title>
    <link rel="stylesheet" href="http://code.jquery.com/ui/1.10.3/themes/base/jquery-ui.css" />
    <script src="http://code.jquery.com/jquery-1.9.1.js"></script>
    <script src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
    <style>
        #draggable {
            width: 125px;
            height: 125px;
            background-color: #FFF;
            text-align: center;
            padding: 1px 5px;
            border: 1px solid #AAA;
            margin: auto;
            float: left;
        }

        #containment-wrapper {
            width: 95%;
            height: 200px;
            border: 1px solid #4E4E4E;
            padding: 10px;
        }
    </style>
    <script>
        $(function() {
            $("#draggable").draggable({
                containment: "#containment-wrapper",
                scroll: false
            });
        });
    </script>
</head>
<body>
    <div id="containment-wrapper">
        <div id="draggable">
            <p>I'm contained within the box</p>
        </div>
    </div>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/af74f8a9-ef7b-476e-8c64-29b548946cdc)   
Kode ini memungkinkan elemen `draggable` dapat dipindahkan (drag) hanya di dalam area `containment-wrapper` menggunakan jQuery UI.   







