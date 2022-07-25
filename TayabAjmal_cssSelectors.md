# Introduction
---
In this article we take a brief look at one type of CSS selectors in order to see how we can use them to create beautiful looking websites and web-based applications. Growing up during the 90's was exiting, epecially around 97-1999 when we got our first desktop computer at home. My teacher gave me some information and said that I could also look up the same information on the internet by searching for a particular address. However, I remember the websites at the time looked terrible, with only some plain HTML where all the elements were stacked on top of each other with some textual information and a few pictures in between. Today, we remember it as the web 1.0.

In today's modern world we have been spoiled with rich functionlity, beautiful looking websites and applications. Being in the industry for more than six years now, working on both customer side and on the vendor side, I notice that end-users are expecting more from business applications. They want the same user-friendliness and rich functionality as they are used to in their private lives; as consumers. This demand certainly requires more competency and skills from developers who are suppose to create the next generation of websites and applications. In fact, in today's world you can even specialize and work on the frontend part of the application and get very good paid. Frontend developers who has an eye for good design and development skills are very much sought after by both startups and big corporations. 

## CSS Selectors
---
It is important to understand how CSS selectors work in terms of syntax and specifity, so that beautiful looking webpages can be created. In order to keep it short and consice, we won't dig much into specificity in this article. 

According to W3Schools CSS selectors can be divided into five categories : 

* Simple selectors (select elements based on name, id, class)
* Combinator selectors (select elements based on specific relationship between them)
* Pseudo-class selectors (select and style based on a certain state)
* Pseudo-elements selectors (select and style a part of an element)
* Attribute selectors (select elements based on an attribute or attribute value)

In this article we will only cover the first category, simple selectors where we select HTML elements based on name, id or class. Let's dig in by writing some HTML and CSS. 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

    <h1>This is some HTML code</h1>
    <h1>This is some more HTML</h1>
    <h1>And this is even more HTML</h1>
    
</body>
</html>
```

I then write the following CSS as well in the head part of the HTML between the opening and closing style tags : 

```
h1 {
        text-align: center;
        color: red;
    }
```

## Select by tagname
---
This will now select all the h1 elements in the HTML document, center them and give them all a red text-color. When we work with CSS selectors we work in two phases. First we select, grap or identify the element using the appropriate CSS syntax. once selected, we style the HTML element by using CSS properties. CSS properties are basically key-value pairs enclosed between curly brackets,  that are made available to us so that we can use them to style our HTML elements. As you continue programming and build muscle memory you will remember the most used HTML tags and CSS properties, but in most cases you will use the internet (google is your friend) to find the properties you are loooking to use in your website/application. 

In the above example we have used CSS selector by name. What if we wanted all our three h1 elements to be differently styled? That is were CSS selector by ID comes in handy. Let's have a look at an example. 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

<style>
    #test1{
        text-align: center;
        color: green;
    }

    #test2{
        text-align: left;
        color: blue;
    }

    #test3{
        text-align: right;
        color: pink;
    }
</style>

</head>
<body>

    <h1 id="test1">This is some HTML code</h1>
    <h1 id="test2">This is some more HTML</h1>
    <h1 id="test3">And this is even more HTML</h1>
    
</body>
</html>
```
## Select by ID
---
In the above example we have given each one of the h1 elements a unique id. We then use, in our CSS in the head, the hash-symbol followed by the id (case sensitive) to select each of the elements. Now we can apply the appropriate CSS properties to style our headings. 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

<style>
    .test1{
        text-align: center;
        color: green;
    }

    .test2{
        text-align: left;
        color: blue;
    }

    .test3{
        text-align: right;
        color: pink;
    }
</style>

</head>
<body>

    <h1 class="test1">This is some HTML code</h1>
    <h1 class="test2">This is some more HTML</h1>
    <h1 class="test3">And this is even more HTML</h1>
    
</body>
</html>
```
## Select by classname
---
In the above code example, we have changed up things a bit. Now, we have given a classname to each one of our h1 elements. We then, in our CSS, use the dot-notation followed by the classname (case sensitive) to style each on of our headings. It is best practise to use ID only for elements that are unique or alone. While, class is used for styling multiple similar elements. 

In this article we have covered how you can use CSS selectors to select and style your HTML elements and make your websites and webapplications look beautiful. 

Thank you for reading.

