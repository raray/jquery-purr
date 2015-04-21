#Instructions on installing and using JQuery Scroll Follow

# Usage #

  1. Include jQuery:
```
  <script type="text/javascript" src="jquery.js"></script>
```
  1. Include Purr:
```
  <script type="text/javascript" src="jquery.purr.js"></script>
```
  1. Build the notice object. This can be done any way you wish, Purr doesn't really care:
```
  <script type="text/javascript">
    var notice = '<div class="notice">'
      + '<div class="notice-body">'
         + '<img src="../static/images/icons/info.png" />'
         + '<h3>Headline</h3>'
         + '<p>Message</p>'
      + '</div>'
      + '<div class="notice-bottom">'
      + '</div>'
    + '</div>';
```
  1. Once the notice is built, simply call Purr on it:
```
    $( notice ).purr();
  </script>
```
  1. Purr accepts several parameters, most of which are adjustments to timing:
```
    $( notice ).purr(
      {
        fadeInSpeed: 200,
        fadeOutSpeed: 2000,
        removeTimer: 5000
      }
    );
  </script>
```
  1. The _isSticky_ parameter allows you to set a notice that won't disapear automatically. Instead the user must manually close a sticky message:
```
    $( notice ).purr(
      {
        isSticky: true,
      }
    );
  </script>
```
  1. The final parameter, _usingTransparentPNG_, should be set to true  if the styling of the notice object is dependent on .png images with transparency. IE7 has issues with combining these images with opacity so Purr will skip the fade in and out animations in IE7:
```
    $( notice ).purr(
      {
        usingTransparentPNG: true,
      }
    );
  </script>
```
  1. All styling of the notice, as well as the structure of the notice itself, happens independently of Purr. Purr only controls the behavior of the notice AS a notice. The two minor exceptions to this are the containing div which uses the id "purr-container," and the close button which has a class of "close." Both of these elements are added through Purr but are styled externally.