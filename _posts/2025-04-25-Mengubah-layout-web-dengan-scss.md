---
layout: post
title: Mengubah Layout Web dengan SCSS.
---

Mengubah Layout Web dengan SCSS.



1. update file navigation.html yang berada didalam folder _includes
```
        <ul>
            {% for item in site.data.navigation %}
            <li>
            <a href="{{ item.link }}" {% if page.url == item.link %} class="active"{% endif %}>
                {{ item.name }}
            </a>
            </li>
            {% endfor %}
        </ul>
```
2. update kode SCSS yang berada pada file main.scss
```
        $primary-color: #b13f57;
        $secondary-color: #f30606;
        $font-stack: Helvetica, sans-serif;

        body,
        h1,
        h2,
        p {
            margin: 0; padding: 0; box-sizing: border-box;
        }

        body {
            font-family: $font-stack; line-height: 1.6;
            background-color: #ffffff;
        }

        header {
            text-align: center; padding: 24px; color: #fff;
            background-color: $primary-color;
        }

        main {
            padding: 24px; margin-top: 24px; color: white;
            box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
            background-color: #966f6f;

        }

        footer {
            text-align: center; padding: 8px; margin-top: 24px; color: #ffffff;
            background-color: $primary-color;
        }

        h2 {
            color: #333; margin-bottom: 8px;
        }

        nav {
            margin: 24px 0;
            ul {
                list-style-type: none; margin: 0; padding: 0; overflow: hidden;
                background-color: $primary-color;
            }
            li {
                float: left;
                a {
                    display: block; color: white; text-align: center; padding: 8px 16px;
                    text-decoration: none;
                    &:hover:not(.active) {
                        background-color: $secondary-color;
                    }
                }
            }
        }

        .container {
            width: 80%; margin: auto; overflow: hidden;
        }

        .profile-picture {
            width: 150px; height: 150px; border-radius: 50%; margin: 24px auto;
            background-color: $secondary-color;
        }

        .active {
            background-color: $secondary-color;
        }
```
3. update file default.html yang berada didalam folder _layouts seperti dibawah ini

```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>{{ page.title }}</title>

            <!--Stylesheet-->
            <link rel="stylesheet" href="{{ site.baseurl }}/assets/css/styles.css">

            <!--Favicon-->
            <link rel="icon" href="{{ site.baseurl }}/assets/images/favicon.ico">

            <!--JavaScript-->
            <script src="{{ site.baseurl }}/assets/js/scripts.js"></script>

            <!--Plugins-->
            {% feed_meta %}
            {% seo %}
```
```
        </head>
        <body>
            <div class="container">
                <header>
                    <img src="{{ site.baseurl }}/assets/images/fotofirdhila.jpg" alt="Profile Picture"
                    class="profile-picture">
                    <h1>{{ site.title }}</h1>
                    <p>{{ site.description }}</p>
                </header>
        <nav>
                    {% include navigation.html %}
                </nav>
                <main>
                    {{ content }}
                </main>

                <footer>
                    <p>&copy; {{ site.time | date: '%Y' }} {{ site.title }}. All rights reserved.</p>
                </footer>
            </div>
        </body>
        </html>
```
