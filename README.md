Nelson,

Put the following inside `assets/scss/base/_fonts.scss1`, but change according to the weights you want to use. The `true` is whether or not to include `.woff2`. 

The `@fonts` includes both regular and italics.

```

$fontfamily: $base-font-family;
$fontpath: "../fonts/${base-font-family}"; //note that $fontpath doesn't require closing slash

@include fonts($fontfamily,$fontpath,100 200 300 400 500 700, true);

```

Then set the `$base-font-family` on line 43 of `assets/scss/abstracts/_variables.scss`:

```
$base-font-family: 'american-sans',avenir,'helvetic neue',helvetica,arial, sans-serif;
```






