# Responsive Menu

Simple responsive menu to slot easily into projects.

It's reasonably flexible with minimal classless markup:
```html
<header>
  <label for="this-id-can-be-anything-you-like"></label>
  <input type="checkbox" id="this-id-can-be-anything-you-like">
  <span>
    <a href="#">Brand</a>
  </span>
  <nav>
    <ul>
      <li><a href="#">Foo</a></li>
      <li><a href="#">Bar</a></li>
      <li><a href="#">Baz</a></li>
    </ul>
    <ul>
      <li>
        <span>user@example.com</span>
      </li>
      <li>
        <logout>Logout</logout>
      </li>
    </ul>
  </nav>
  <menu-open></menu-open>
  <menu-close></menu-close>
</header>
```


Set the breakpoint at the screen size you wish to cap the mobile menu:
```css
...

@media (max-width: 576px) {

...

```

The menu scales pretty well, only the following two variables really need to be changed:

```css
--brand-height: 2rem;
--menu-right-width: 10rem;

```

The main font is 60 per cent of the `--brand-height` variable but this can be changed if desired.
The `--menu-right-width` may need to be adjusted to cater for the size of any right-sided text.
This menu was tested in all modern browsers and there were no issues.
