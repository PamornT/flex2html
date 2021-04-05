# flex2html - Convert LINE Flex message to HTML

## How to use

- **include CSS file**
```
<link rel="stylesheet" href="css/flex2html.css" >
```

- **include JS file**
```
<script type="text/javascript" src="js/flex2html.min.js"></script>
```

- **create layer element**
```
<div id="flex1"></div>
```

- **call function**

```
flex2html(elementId, flexJson)
```

**Example**
```
flex2html("flex1", {"type":"flex","altText":"Flex Message","contents": {"type":"carousel", ……}})
```