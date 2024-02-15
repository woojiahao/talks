# talks

Repository for slides for workshops that I've given/going to give!

## Template used

I have added some customization for my slides:

```yaml
marp: true
theme: uncover
class:
    - invert
    - modern
style: |
  .left-heavy-two-column {
    display: grid;
    grid-template-columns: 1fr 3fr;
    gap: 1rem;
  }

  .even-two-column {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0.3rem;
  }
```

I created a custom layout to split a slide into two.

I also use Mermaid to generate diagrams. Add this to the top of markdown file:

```javascript
<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
  mermaid.initialize({
    startOnLoad: true,
    theme: 'dark'
  });
</script>
```

## Exporting

```
marp slides.md --html -o slides.pdf --allow-local-files
```
