##Website Performance Optimization portfolio project

###Objective:

To optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible.

### Getting started

####Setup: Optimize PageSpeed Insights score for index.html


1. Download the repository

2. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

3. Open a browser and visit localhost:8080

4. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
  ```

### After establishing the connection the Tunnel will be active

5. Copy the public URL ngrok gives you and run it through PageSpeed Insights! measuring Profile, optimizing it, and then lather, rinse, and repeat. 

####Part 1: Optimize PageSpeed Insights score for index.html

1. Checked PageSpeed Insight for score on mobile and desktop devices.

2. Recorded the timeline using Devtools to figure out jank.

3. Reduced the image sizes using adobe photoshop.

4. Added media=“print” to stop render blocking CSS

5. Inlined style “text/css” in index.html

6. Added script async for GoogleAnalytics

7. Shifted all JS to the bottom of the page to improve load time

####Part 2: Optimize Frames per Second in pizza.html

1. Recorded the timeline using Devtools to figure out jank.

2. Changed querySelector where used to getElementById because it is a faster method

3. Made changes in UpdatePosition(), changePizzaSizes(), and elem to have dynamic characteristics 

4. Added comments for easy understanding.

5. minified the JavaScript file.


### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>