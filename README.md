# flex2html - Convert LINE Flex message to HTML

## How to use

- **include CSS file**
```
<link rel="stylesheet" href="css/flex2html.css">
```

- **include JS file**
```
<script type="text/javascript" src="js/flex2html.min.js"></script>
```

- **create HTML layer element**
```
<div id="flex1"></div>
```

- **call function**

```
flex2html(elementId, flexJson)
```

## Example
```
<html>
   <head>
      <link rel="stylesheet" href="css/flex2html.css" >
      <script type="text/javascript" src="js/flex2html.min.js"></script>
   </head>
   <body>
      
      <div class="chatbox">
         <div id="flex1"></div>
      </div>
      
      <script>
         const target_element = "chatbox"
         flex2html{
  "line": {
    "type": "flex",
    "altText": "พื้นหลังแบบเบลอ",
    "contents": {
      "type": "carousel",
      "contents": [
        {
          "type": "bubble",
          "body": {
            "type": "box",
            "layout": "vertical",
            "contents": [
              {
                "type": "image",
                "url": "https://picsum.photos/1040/1040/?blur=8",
                "size": "full",
                "aspectMode": "cover",
                "aspectRatio": "1:1",
                "gravity": "top"
              },
              {
                "type": "box",
                "layout": "vertical",
                "contents": [
                  {
                    "type": "box",
                    "layout": "vertical",
                    "contents": [
                      {
                        "type": "text",
                        "text": "Sally The Rock",
                        "size": "xl",
                        "color": "#ffffff",
                        "weight": "bold",
                        "align": "center",
                        "wrap": true
                      }
                    ],
                    "backgroundColor": "#00a30055",
                    "cornerRadius": "md",
                    "borderColor": "#00a300",
                    "borderWidth": "3px"
                  },
                  {
                    "type": "box",
                    "layout": "vertical",
                    "contents": [
                      {
                        "type": "filler"
                      },
                      {
                        "type": "box",
                        "layout": "baseline",
                        "contents": [
                          {
                            "type": "filler"
                          },
                          {
                            "type": "text",
                            "text": "CLICK",
                            "color": "#ffffff",
                            "offsetTop": "-2px"
                          },
                          {
                            "type": "filler"
                          }
                        ],
                        "spacing": "sm"
                      },
                      {
                        "type": "filler"
                      }
                    ],
                    "borderWidth": "1px",
                    "cornerRadius": "4px",
                    "spacing": "sm",
                    "borderColor": "#ffffff",
                    "margin": "xxl",
                    "height": "40px",
                    "backgroundColor": "#4d4d4d55",
                    "action": {
                      "type": "uri",
                      "label": "action",
                      "uri": "https://picsum.photos/1040/1040/?blur=8"
                    }
                  }
                ],
                "position": "absolute",
                "offsetBottom": "0px",
                "offsetStart": "0px",
                "offsetEnd": "0px",
                "paddingAll": "20px",
                "paddingTop": "18px",
                "offsetTop": "100px"
              },
              {
                "type": "box",
                "layout": "vertical",
                "contents": [
                  {
                    "type": "image",
                    "url": "https://sv1.picz.in.th/images/2021/08/04/2qQv8n.png",
                    "animated": true,
                    "size": "full"
                  }
                ],
                "position": "absolute",
                "cornerRadius": "150px",
                "offsetTop": "18px",
                "offsetStart": "18px",
                "height": "80px",
                "width": "80px"
              }
            ],
            "paddingAll": "0px"
          }
        }
      ]
    }
  }
}
      </script>
   </body>
</html>
```
