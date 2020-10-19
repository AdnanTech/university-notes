# Web Activity Worksheets 2

## [Questions](https://github.com/AdnanTech/UniversityOfSussex/blob/master/ComputingProject/WebActivityWorksheet2.pdf)

### Do HTML tags always come in pairs?

No, some are self closing, and dont need a pair, for example &lt;meta/&gt;

### Provide an example of HTML element with at least one suitable attribute and value

&lt;img src="hello\_world.jpg"&gt;, where the attribute is src="hello\_world.jpg", attribute name is img, and the attirubte value is hello\_world.jpg

### Do All HTML attributes requires name and a value?

Yes, even if empty, still a value is required

### HTML and relevant attributes should be used to format all page content

Yes, this helps the browers format so they can show the webpage to you, and helps you edit the webpage in the future if necessary

{% tabs %}
{% tab title="Summary" %}
```
Table Practice
```
{% endtab %}

{% tab title="HTTP" %}
{% code title="tableBasics" %}
```http
<!DOCTYPE html>

<html lang="en">
<head>

    <!-- Meta
    ============================================= -->
    <meta http-equiv="content-type" content="text/html; charset=utf-8" />
	<meta name="author" content="AdnanQuisar" />

    <!-- Stylesheets
	  ============================================= -->
    <link rel="stylesheet" type="text/css" href="style/style.css" title="style" />

    <!-- Document Title
    ============================================= -->
    <title>Web Activity</title>
</head>

<body>

   	<!-- Content
   	============================================= -->
    
    <!-- Question A -->
    <table border="1">
        <tbody>
            <tr>
                <td>One</td>
                <td>Two</td>
            </tr>
            
            <tr>
                <td>Three</td>
                <td>Four</td>
            </tr>
        </tbody>
    </table>
   
    <br><br>

    <!-- Question B -->
    <table border="1">
        <tbody>
            <tr>
                <td><b>Day</b></td>
                <td><b>Start</b></td>
                <td><b>End</b></td>
            </tr>
            
            <tr>
                <td><b>Monday</b></td>
                <td>10:00</td>
                <td>18:00</td>
            </tr>

            <tr>
                <td><b>Tuesday</b></td>
                <td>09:00</td>
                <td>17:00</td>
            </tr>
        </tbody>
    </table>

    <br><br>

    <!-- Question C -->
    <table border = "1">
        <tbody>
            <tr>
            <td><b>Kinglsey</b></td>
            <td colspan="2"><b>Ramiz</b></td>
            <td><b>Richard</b></td>
            </tr>
            
            <tr>
            <td>Mathematics for Computing 1</td>
            <td>Communication and Learning Skills</td>
            <td>Computing Project</td>
            <td>Foundation Programming</td>
            </tr>
        </tbody>
    </table>

    <br><br>

    <!-- Question D -->
    <table border = "1">
        <tbody>
            <tr>
            <td><b>Richard</b></td>
            <td>Foundation Programming</td>
            </tr>

            <tr>
                <td rowspan="2"><b>Ramiz</b></td>
                <td>Communication and Learning Skills
            </tr>

            <tr>
                <td>Computing Project</td>
            </tr>
            
            <tr>
                <td><b>Kinglsey</b></td>
                <td>Mathematics for Computing 1</td>
            </tr>
        </tbody>
    </table>

    <br><br>

    <!-- Question E -->
    <table border = "1">

        <tbody>
            <tr>
                <td colspan="2">
                    Nested Table
                    <table border="1" width>
                        <tbody>
                            <tr>
                                <td>Top Left</td>
                                <td>Top Right</td>
                            </tr>
                            
                            <tr>
                                <td>Bottom Left</td>
                                <td>Bottom Right</td>
                            </tr>

                            
                        </tbody>
                    </table>
                </td>
            </tr>

            <tr>
                <td>
                    An ordered list
                    <ol type="i">
                        <li>One</li>
                        <li>Two</li>
                        <li>Three</li>
                    </ol>
                </td>
                    
                <td>
                    Nested lists
                    <br><br>
                    Fruit and Veg list
                    <ul>
                        <li>Fruit</li>
                        <ol>
                            <li>Tomato</li>
                            <li>Apple</li>
                            <ul>
                                <li>Bramley</li>
                                <li>Gala</li>
                            </ul>
                        </ol>

                        <li>Vegetable</li>
                        <ol>
                            <li>Potato</li>
                        </ol>
                    </ul>
                </td>
            </tr>


            <tr>
                
                <td colspan="2">Definition list
                    <br><br>
                    HTML
                    <br>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; HyperText Markup Language is...
                </td>
            </tr>

        </tbody>
    </table>

    <br><br>
    
    <a href="http://www.bbc.co.uk" target="_blank">BBC website</a>


</body>
</html>
```
{% endcode %}
{% endtab %}
{% endtabs %}

