# BootstrapButtons

## Learning Objectives
* Using bootstrap button styles

## The Walkthrough

1. Create a Spring Boot Application
	* Name it BootsrapButtons
	* Add the dependencies for the web and for thymeleaf
	* Hit next until you finish the wizard, and then wait until it's done.

2. Create a Controller
	* Right click on com.example.demo and click New -> Class
	* Name it HomeController.java
	* Edit it to look like this:
```java
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class HomeController {

    @RequestMapping("/")
    public String index(){
        return "index";
    }
}
```

3. Create a Template
  * Right click on templates and click New -> Html
	* Name it index.html
	* Edit it to look like this:
```html
<!DOCTYPE html>
<html lang="en" xmlns:th="www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title>Bootstrap 101 template</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
</head>
<body>
<div class="container">
    <br>
    <h1>Buttons in Bootsrap</h1>
    <h2>Button Styles</h2>
    <button type="button" class="btn btn-primary ">Primary</button>
    <button type="button" class="btn btn-secondary">Secondary</button>
    <button type="button" class="btn btn-success">Success</button>
    <button type="button" class="btn btn-danger">Danger</button>
    <button type="button" class="btn btn-warning">Warning</button>
    <button type="button" class="btn btn-info">Info</button>
    <button type="button" class="btn btn-light">Light</button>
    <button type="button" class="btn btn-dark">Dark</button>
    <button type="button" class="btn btn-link">Link</button>
    <h2>Outline Buttons</h2>
    <button type="button" class="btn btn-outline-primary">Outline</button>
    <h2>Sizes</h2>
    <button type="button" class="btn btn-primary btn-lg">Large</button>
    <button type="button" class="btn btn-primary btn-md">Medium</button>
    <button type="button" class="btn btn-primary btn-sm">Small</button>
    <h2>Disabled/ Active state</h2>
    <button type="button" class="btn btn-primary disabled">Disabled</button>
    <button type="button" class="btn btn-primary active">Active</button>
</div>
</body>
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</html>
```

4. Run your application and open a browser, if you type in the URL http://localhost:8080 you should see this:
![](https://github.com/ajhenley/unofficialguides/blob/master/IntroToSpringBoot/img/Lesson11.png)

## What is Going On

### The Controller
Here, the default route maps to index.html.

### The View
Bootstrap includes several predefined button styles.
btn - class is a basic class for creating button.
Elements that you can use button classes are <a>, and <button> tags, and <input> field.
To specify the color you can type btn- and choose any of the available colors (eg. - btn-primary). There are 8 different colors you can choose from.

#### Outline buttons
Replacing the default modifier classes with the .btn-outline removes all background images and colors on any button.

#### Sizes
To change button sizes to large use btn-lg or use btn-sm for smaller button sizes.

#### States
active and disabled classes
By adding active or disabled class makes button look active or inactive.

