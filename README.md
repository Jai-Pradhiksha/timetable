# Ex03 Time Table
## Date: 02.04.2024

## AIM
To write an HTML webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create a static folder and insert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html.

### STEP 4
Add header row using ```<th>``` tag.

### STEP 5
Add your timetable using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">

<head>
    {% load static %}
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jai Pradhiksha</title>
    <style>
        table,
        th,
        td {
            border: 1px solid black;
            border-style: double;
            text-align: center;

        }

        .td1 {
            background-color: aqua;
        }

        .td2 {
            background-color: yellow;
        }

        table,
        img,
        h3 {
            margin-left: auto;
            margin-right: auto;
        }
    </style>
</head>

<body>
    <div class="col-6 mx-auto">
        <img src="{% static 'images/logo.png'%}" alt="">
        <h3 style="text-align: center;">SLOT TIME TABLE - JAI PRADHIKSHA D P (212221040062)</h3>
    </div>
    <div class="col-6 mx-auto">
        <table>
            <tr class="td2">
                <th>Day/Time</th>
                <th>Monday</th>
                <th>Tuesday</th>
                <th>Wednesday</th>
                <th>Thursday</th>
                <th>Friday</th>
            </tr>
            <tr>
                <td class="td2"><b>8-10</b></td>
                <td colspan="3" class="td1">FREE SLOT</td>
                <td class="td1">PHY</td>
                <td class="td1">CHE</td>
            </tr>
            <tr>
                <td class="td2"><b>10-12</b></td>
                <td class="td1">GER</td>
                <td class="td1">FREE SLOT</td>
                <td class="td1">FWAD</td>
                <td class="td1">FWAD</td>
                <td class="td1">PHY</td>
            </tr>
            <tr>
                <td class="td2"><b>12-1</b></td>
                <td colspan="5" class="td1">LUNCH</td>
            </tr>
            <tr>
                <td class="td2"><b>1-3</b></td>
                <td colspan="2" class="td1">FREE SLOT</td>
                <td class="td1">MAT</td>
                <td class="td1">MAT</td>
                <td class="td1">SS</td>
            </tr>
            <tr>
                <td class="td2"><b>3-5</b></td>
                <td colspan="2" class="td1">FREE SLOT</td>
                <td class="td1">GER</td>
                <td class="td1">CHE</td>
                <td class="td1">FWAD</td>
            </tr>
        </table>

    </div>
    <br>
    <div class="col-6 mx-auto">
        <table>
            <tr>
                <th>S.No.</th>
                <th>Subject Code</th>
                <th>Subject Name</th>
            </tr>
            <tr>
                <td>1.</td>
                <td>19AI414</td>
                <td>Fundamentals of Web Application Development (FWAD)</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>19EN612</td>
                <td>German Basic (GER)</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>19PH206</td>
                <td>Physics for Information Technology (PHY)</td>
            </tr>
            <tr>
                <td>4.</td>
                <td>19CY205</td>
                <td>Principles of Chemistry in Engineering (CHE)</td>
            </tr>
            <tr>
                <td>5.</td>
                <td>19MA201</td>
                <td>Calculus and Matrix Algebra</td>
            </tr>
            <tr>
                <td>6.</td>
                <td>19EY701</td>
                <td>Soft Skills</td>
            </tr>

        </table>
    </div>
</body>

</html>
```

## OUTPUT
![image](https://github.com/Jai-Pradhiksha/timetable/assets/100289733/71398bd5-ba01-462e-a642-69a309b7bcf0)


## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
