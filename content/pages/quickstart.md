
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أسئلة نعم أو لا</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            padding: 20px;
        }
        .question {
            margin: 20px 0;
            font-size: 18px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #45a049;
        }
        .answer {
            font-size: 20px;
            margin-top: 10px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>أسئلة نعم أو لا</h1>
    
    <div class="question">
        <p>هل تحبيني؟</p>
        <button onclick="askQuestion(1)">اسأل</button>
        <div id="answer1" class="answer"></div>
    </div>
    
    <div class="question">
        <p>هل تريدين أن تكوني فالنتين؟</p>
        <button onclick="askQuestion(2)">اسأل</button>
        <div id="answer2" class="answer"></div>
    </div>
    
    <div class="question">
        <p>هل تريدين أن نبقى مع بعض للأبد؟</p>
        <button onclick="askQuestion(3)">اسأل</button>
        <div id="answer3" class="answer"></div>
    </div>

    <script>
        function askQuestion(questionNumber) {
            const answers = ["نعم", "لا"];
            const randomAnswer = answers[Math.floor(Math.random() * answers.length)];
            document.getElementById('answer' + questionNumber).textContent = randomAnswer;
        }
    </script>
</body>
</html><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>أسئلة نعم أو لا</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f0f0f0;
            padding: 20px;
        }
        .question {
            margin: 20px 0;
            font-size: 18px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #45a049;
        }
        .answer {
            font-size: 20px;
            margin-top: 10px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>أسئلة نعم أو لا</h1>
    
    <div class="question">
        <p>هل تحبيني؟</p>
        <button onclick="askQuestion(1)">اسأل</button>
        <div id="answer1" class="answer"></div>
    </div>
    
    <div class="question">
        <p>هل تريدين أن تكوني فالنتين؟</p>
        <button onclick="askQuestion(2)">اسأل</button>
        <div id="answer2" class="answer"></div>
    </div>
    
    <div class="question">
        <p>هل تريدين أن نبقى مع بعض للأبد؟</p>
        <button onclick="askQuestion(3)">اسأل</button>
        <div id="answer3" class="answer"></div>
    </div>

    <script>
        function askQuestion(questionNumber) {
            const answers = ["نعم", "لا"];
            const randomAnswer = answers[Math.floor(Math.random() * answers.length)];
            document.getElementById('answer' + questionNumber).textContent = randomAnswer;
        }
    </script>
</body>
</html>
## Changing the title and description

By default, the title of your site is `username.github.io`. You can change the title by editing the `_config.yml` file in your repository. You can also add a description for your site.

1. Click the **Code** tab of your repository.
1. In the file list, click `_config.yml` to open the file.
1. Click {% octicon "pencil" aria-label="The edit icon" %} to edit the file.
1. The `_config.yml` file already contains a line that specifies the theme for your site. Add a new line with `title:` followed by the title you want. Add a new line with `description:` followed by the description you want. For example:

   ```yaml
   theme: jekyll-theme-minimal
   title: Octocat's homepage
   description: Bookmark this to keep an eye on my project updates!
   ```

1. When you are finished editing the file, click **Commit changes**.

## Next Steps

You've successfully created, personalized, and published your first {% data variables.product.prodname_pages %} website but there's so much more to explore! Here are some helpful resources for taking your next steps with {% data variables.product.prodname_pages %}:

* [AUTOTITLE](/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll#about-content-in-jekyll-sites): This guide explains how to add additional pages to your site.
{% ifversion fpt or ghec %}* [AUTOTITLE](/pages/configuring-a-custom-domain-for-your-github-pages-site): You can host your site on {% data variables.product.prodname_dotcom %}'s `github.io` domain or your own custom domain.{% endif %}
