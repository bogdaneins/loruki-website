### Navbar

```htnl
<div class="navbar">
  <div class="container flex">
    <h1 class="logo">Loruki.</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="features.html">Features</a></li>
        <li><a href="docs.html">Docs</a></li>
      </ul>
    </nav>
  </div>
</div>
```

```css
:root {
  --primary-color: #047aed;
}

ul {
  list-style-type: none;
}

.navbar {
  background-color: var(--primary-color);
  color: #fff;
  height: 70px;
}

.navbar .flex {
  justify-content: space-between;
}

.navbar ul {
  display: flex;
}

.navbar a {
  color: #fff;
  padding: 10px;
  margin: 0 5px;
}

.navbar a:hover {
  border-bottom: 2px solid #fff;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  overflow: auto;
  padding: 0 40px;
}
```

### Justify a form, inside its container, to the right

```css
.showcase-form {
  position: relative;
  top: 60px;
  height: 350px;
  width: 400px;
  padding: 40px;
  z-index: 100;
  justify-self: flex-end;
}
```

### Showcase with fixed width form and text description

```html
<section class="showcase">
  <div class="container grid">
    <div class="showcase-text">
      <h1>Easier Deployment</h1>
    </div>
    <div class="showcase-form">
      <form>
        <input>
        <input>
        <input>
        <submit>
      </form>
    </div>
  </div>
</section>
```

```css
.showcase {
  position: relative;
  height: 400px;
  background-color: var(--primary-color);
  color: #fff;
}

.showcase .grid {
  overflow: visible;
  grid-template-columns: 55% auto; // auto maintains text description alignement vs. a value like 45%
  gap: 30px;
}

.showcase-form {
  position: relative;
  top: 60px;
  height: 350px;
  width: 400px;
  padding: 40px;
  z-index: 100;
  justify-self: flex-end;
}
```
