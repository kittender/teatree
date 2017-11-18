# Teatree
Organize your code along **a logical architecture**.  
*Cascading the right way*, in the right **order of prevalence**.  

Inspired by [ITCSS](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/).

##### __φ(．．)

* @todo : add layer management infos

### Vendor
**00_vendor** | For libraries and external sources

*Example :* 
```
/framework.css
/normalize.css
```

### Settings
**01_settings** | For configuration and variables

*Example :* 
```
/variables.less
/layers.less
/theme.less
```

### Tools
**02_tools** | For functions, mixins and utilities

*Example :* 
```
/mixins.less
/functions.less
/utils.css
```

### Generic
**03_generic** | For globals and wild cards

*Example :* 
```
/reset.css
/set.css
/print.css
```

### Elements
**04_elements** | For bare tag styles

*Example :* 
```
/body.css
/anchor.css
/paragraph.css
/mark.css
/heading.css
```

### Objects
**05_objects** | For layout components

*Example :* 
```
/header.css
/navigation.css
/media.css
/footer.css
```

### Components
**06_components** | For reusable components

*Example :* 
```
/popin.css
/popover.css
/dropdown.css
/article.css
/tooltip.css
```

### Modules
**07_modules** | For unique areas and pages

*Example :* 
```
/homepage.css
/profile.css
/shop.css
/payment.css
```