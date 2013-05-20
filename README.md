# Radio DePaul API

Radio DePaul provides jsonp resources for cross-domain access.

Be sure to specify a ```jsonp``` dataType and an ```application/json``` contentType.

All API access is over HTTP and accessed over the radiodepaul.herokuapp.com/api domain. All data should be sent and received as JSON.

```javascript
$.ajax({
  url: 'http://radiodepaul.herokuapp.com/api/resource.js',
  dataType: 'jsonp',
  type: 'GET',
  contentType: 'application/json',
  success: function(data) {
    // do something
  }
});
```
