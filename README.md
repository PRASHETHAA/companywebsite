# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title> Prash Corp Limited </title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/c img.jpg' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Prash Corp Limited
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contactus">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2021 venus Private Limited, Developed by Prashethaa Ramkumar
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/c img.jpg" alt="Building">
    <div class="contenttext">
    Prash Corp Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="productcontent">
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/DDR4 RAM.jpeg" alt="product image">
            </div>
            <div class="itemname">DDR4 RAM</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/TOSHIBA 1TB.jpeg" alt="product image">
            </div>
            <div class="itemname">TOSHIBA 1TB</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/graphics card.jpeg" alt="product image">
            </div>
            <div class="itemname">Graphics card</div>
            <div class="itemprice">Price: Rs.30000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/mouse.jpg" alt="product image">
            </div>
            <div class="itemname">Mouse</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/cabinet.jpeg" alt="product image">
            </div>
            <div class="itemname">Cabinet</div>
            <div class="itemprice">Price: Rs.25000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/RAM.jpg" alt="product image">
            </div>
            <div class="itemname">RAM</div>
            <div class="itemprice">Price: Rs.4000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/keyboard.jpg" alt="product image">
            </div>
            <div class="itemname">Keyboard</div>
            <div class="itemprice">Price: Rs.2500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/SATA SSD.jpg" alt="product image">
            </div>
            <div class="itemname">SATA SSD (samsung)</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/web cam.jpeg" alt="product image">
            </div>
            <div class="itemname">Web cam</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/motherboard.jpeg" alt="product image">
            </div>
            <div class="itemname">Motherboard</div>
            <div class="itemprice">Price: Rs.10000.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/SATA HDD.jpg" alt="product image">
            </div>
            <div class="itemname">SATA HDD</div>
            <div class="itemprice">Price: Rs.5500.00 </div>
        </div>
        <div class="productitem">
            <div class="itemimage">
                <img src="/static/img/RYZEN 7 3700X.jpg" alt="product image">
            </div>
            <div class="itemname">RYZEN 7 3700x processor</div>
            <div class="itemprice">Price: Rs.36000.00 </div>
        </div>
    </div>
</div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
    <h1>Our Crew</h1>
    <div class="crewmembers">
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/prashethaa.jpeg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">PRASHETHAA RAMKUMAR</div>
            <div class="designation">C.E.O PRASH CORP</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/nissetha.jpeg" alt="member image" style="width:200px;height:200px;>
            </div>
            <div class="membername">NISSETHA</div>
            <div class="designation">FRONTEND DEV</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ananditha.jpeg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">ANANDITHA</div>
            <div class="designation">TECHNICAL TEAM</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/kishan.jpeg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">KISHAN</div>
            <div class="designation"> R & D HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ranjini.jpeg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">RANJINI</div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/pooja.jpeg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">POOJA</div>
            <div class="designation"> MARKETING HEAD </div>
        </div>
    </div>
    {% endblock  %}
```
### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
<form action="//submit.form" id="ContactUs100" method="post" onsubmit="return ValidateForm(this);">
<script type="text/javascript">
function ValidateForm(frm) {
if (frm.Name.value == "") { alert('Name is required.'); frm.Name.focus(); return false; }
if (frm.FromEmailAddress.value == "") { alert('Email address is required.'); frm.FromEmailAddress.focus(); return false; }
if (frm.FromEmailAddress.value.indexOf("@") < 1 || frm.FromEmailAddress.value.indexOf(".") < 1) { alert('Please enter a valid email address.'); frm.FromEmailAddress.focus(); return false; }
if (frm.Comments.value == "") { alert('Please enter comments or questions.'); frm.Comments.focus(); return false; }
return true; }
</script>
<table style="width:100%;max-width:550px;border:0;" cellpadding="8" cellspacing="0">
<tr> <td>
<label for="Name">Name*:</label>
</td> <td>
<input name="Name" type="text" maxlength="60" style="width:100%;max-width:250px;" />
</td> </tr> <tr> <td>
<label for="PhoneNumber">Phone number:</label>
</td> <td>
<input name="PhoneNumber" type="text" maxlength="43" style="width:100%;max-width:250px;" />
</td> </tr> <tr> <td>
<label for="FromEmailAddress">Email address*:</label>
</td> <td>
<input name="FromEmailAddress" type="text" maxlength="90" style="width:100%;max-width:250px;" />
</td> </tr> <tr> <td>
<label for="Comments">Comments*:</label>
</td> <td>
<textarea name="Comments" rows="7" cols="40" style="width:100%;max-width:350px;"></textarea>
</td> </tr> <tr> <td>
* - required fields
</td> <td>
<input name="skip_Submit" type="submit" value="Submit" />
</td> </tr>
</table>
</form>
{% endblock  %}
```
## OUTPUT:
![output](./static/img/output1.png)

![output](./static/img/output2.png)

![output](./static/img/output.3png)

![output](./static/img/output4.png)

## CODE VALIDATION REPORT:
![output](./static/img/base validator.jpeg)

![output](./static/img/home validator.jpeg)

![output](./static/img/product validator.jpeg)

![output](./static/img/people validator.jpeg)

![output](./static/img/contactus validator.jpeg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://prashethaa.student.saveetha.in:8000/. HTML code is validated.