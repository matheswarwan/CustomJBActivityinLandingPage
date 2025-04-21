# CustomJBActivityinLandingPage

The idea goes like this.

1. Index page hosted in say below URL 
https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/ytvlbcz4o3d

2. In installed package, give this url - note that additional ?f= that defines the file name 
https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/ytvlbcz4o3d?f=

3. In the index page, read the f parameter 
var fileName = RequestParameter('f');

4. If fileName is available, then RedirectTo that url. Eg., on load, config.json will be requested.
Requested: https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/ytvlbcz4o3d?f=config.json 
Redirect to: https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/pecgailcewe - which is a config.json 

5. similarly, have other files as well available..

var redirectUrls = {
    'config.json' : 'https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/pecgailcewe',
    'customActivity.js' : 'https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/tvjeffdlbr4',
    'jquery.min.js' : 'https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/cquiaqnf2r2',
    'require.js' : 'https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/q2dt4ukkvz0',
    'postmonger.js' : 'https://mc-yfyyj2sjhsjhkwc1s8w4zrxx4.pub.sfmc-content.com/4ly1prpqabw'
}