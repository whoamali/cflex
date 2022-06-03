# CFlex
A CSS library for responsive design using flex-box

Fast - Light - Simple

<p align="center"><img src="/images/Examples.png" data-canonical-src="/images/Examples.png" width="500" /></p>

## Installation
you can download css files or clone this repository!

```bash
git clone https://github.com/whoamali/cflex.git
```

## Usage
reference css file to your html

```html
<link rel="stylesheet" href="./ltr/cflex.css">
<link rel="stylesheet" href="./ltr/cflex.min.css">
<link rel="stylesheet" href="./rtl/cflex-rtl.css">
<link rel="stylesheet" href="./rtl/cflex-rtl.min.css">
```

#### Class
add ``cflex`` class to your container element to add CFlex styles styles

```html
<div class="cflex">
  ...
</div>
```

now you can use cflex columns

```html
<div class="cflex">
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
  <div class="c-1"></div>
</div>
```

**Each container is divided into 10 parts**

You can use c-1 to c-10

In this case, the children stick to each other! If you do not want this to happen, use ``cm``

```html
<div class="cflex">
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
</div>
```

You can use ``off-[1-10]`` to distance the children

```html
<div class="cflex">
  <div class="cm-1 off-2"></div>
  <div class="cm-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1 off-1"></div>
  <div class="cm-1"></div>
  <div class="cm-1 off-1"></div>
</div>
```

You can centered elements with ``centered`` class
```html
<div class="cflex centered">
  <div class="cm-1"></div>
  <div class="cm-5"></div>
</div>
```

**You can use s, md, lg, xl, xxl, xxxl sizes to be responsive and have control on different screens.**

```
375  >= normal # Normal means without any writing
425  >= s      > 375
768  >= md     > 425
1024 >= lg     > 768
1440 >= xl     > 1024
2560 >= xxl    > 1440
        xxxl   > 2560
```
```
centered-[normal-xxxl]
c-[normal-xxxl]-[1-10]
cm-[normal-xxxl]-[1-10]
off-[normal-xxxl]-[1-10]
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
