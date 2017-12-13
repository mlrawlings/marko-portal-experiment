# A Portal Component for Marko

By default, the portal renders into `document.body`:
```marko
<portal>
   ...content here...
</portal>
```

You can set a custom target using a DOM id:
```marko
<portal target="some-id">
   ...content here...
</portal>
```

Or by passing a DOM Node:
```marko
<portal target=someNode>
   ...content here...
</portal>
```

# Demo

Run `npm start` to start the server and visit `http://localhost:8080/`

The `<counter>` component uses `<portal>` to put a portal that includes the count at the bottom of the page (scroll down).  When the count reaches 3, it will move into the first section (`id="first"`) and when the count reaches 10, it will be removed.