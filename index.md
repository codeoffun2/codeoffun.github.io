## Welcome to GitHub Pages

//initial number of cookies    
var num = 0;

window.onload = function () {
        var name = prompt("What is your name");
        
        var space = document.getElementById("space");
        
        space.innerHTML = name + "'s Bakery";
}

var cookie = document.getElementById("cookie");

function cookieClick() { 
    num += 1;

    var numbers = document.getElementById("numbers");
    
    //upgrade level for printing
    var upgradeLevel = document.getElementById("upgradeLevel");
    
    numbers.innerHTML = num;      
    //automatic Granny upgrade to 2x
    if(num >= 30 ){
        num += 2;
        upgradeLevel.innerHTML = "Granny Level";
    }

    //automatic factory upgrade to 10x
    if(num >= 500) {
        num += 10;
        upgradeLevel.innerHTML = "Factory Level";
    }

    //automatic plant upgrade to 30x
    if(num >= 1000) {
        num += 30;
        upgradeLevel.innerHTML = "Plant Level";
    }

    //automatic super factory upgrade to 1000x
    if(num >= 100000) {
        num += 1000;
        upgradeLevel.innerHTML = "Super-Plant Level";
    }
}
### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/codeoffun2/codeoffun.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
