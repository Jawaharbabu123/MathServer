# Ex.05 Design a Website for Server Side Processing
## Date: 30-11-2024

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```

<!DOCTYPE html>
<html>
<head>
    <title>Power</title>
    <style>
        *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body{
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: cursive;
    background-color: antiquewhite;
    background-size: cover;
} 
h1{
    margin-bottom: 30px;
    text-align: center;
}
.container{
    background-color:gray;
    padding: 50px;
    width: 35%;
    margin-top: 175px;
}
.inputline{
    display: flex;
    height: 40px;
    margin-top: 10px;
    justify-content: space-between;
}

    </style>
</head>

<body>
    <div class="container">
        <h1>Power Calculator</h1>
        <form method="post">
            {% csrf_token %}
            <div class="inputline">
                Resistance : <input type="text" name="Resistance" placeholder="Enter Resistance(in ohms)" value="{{R}}"></input></br>
            </div>
            <div class="inputline">
                Resistance : <input type="text" name="Intensity" placeholder="Enter Intensity" value="{{I}}"></input></br>
            </div>
            <div>
                <div class="inputline">
                    <input type="submit" value="Calculate"></input></br>
                </div>
            </div>
            <div class="inputline">
                Power : <input type="text" name="Power" placeholder="Power calculated" value="{{power}}"></input></br>

            </div>
        </form>
    </div>
</body>

</html>
```

## SERVER SIDE PROCESSING:

![Screenshot (40)](https://github.com/user-attachments/assets/4519fda1-2465-4aca-8414-956c64a1c1e9)

## HOMEPAGE:

![Screenshot (39)](https://github.com/user-attachments/assets/3c96df28-ec12-496b-8ea4-d11b1b7d7f03)


## RESULT:
The program for performing server side processing is completed successfully.
