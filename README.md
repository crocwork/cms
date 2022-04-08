# Lottie

This __October CMS__ plugin allows to add Lottie animations on your website with ease.

![og-image](https://github.com/croqo/oc-lottie-plugin/blob/dev/sources/og-image.png)

🤔 [What is Lottie?](https://lottiefiles.com/what-is-lottie)

## Component Player

Use this code in INI section to inject JS player into current page/partial/layout.

```ini
[lottie]
```

When it's done, you can use Lottie player as many times as you want with different values of **url** property.

+ ### url

    HTTP link to lottie animation json.

    Next example code will generate two animations following one-by-one:

    ```twig
    {% component 'lottie' url='https://path.to/file1.json' %}

    {% component 'lottie' url='https://path.to/file2.json' %}
    ```

+ ### look

    Lottie player CSS style
    
    ```twig
    {% component 'lottie' url='https://path.to/file.json' look='custom-css-style' %}}
    ```
    
+ ### ratio

    preserveAspectRatio option (rendererSettings)
    
    ```twig
    {% component 'lottie' url='https://path.to/file.json' ratio='xMidYMid slice' %}}
    ```
