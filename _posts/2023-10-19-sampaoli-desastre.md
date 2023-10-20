## Sampaoli é um desastre

<iframe id="iframeElement" sandbox="allow-same-origin allow-scripts" width="100%" height="600" scrolling="no" seamless="seamless" frameborder="0"></iframe>

<script>
    // Function to check the browser window width and change iframe source
    function checkWindowWidth() {
        var width = window.innerWidth || document.documentElement.clientWidth || document.body.clientWidth;
        var iframeElement = document.getElementById("iframeElement");

            if (width > 1800) {
                iframeElement.src = "/Assets/Bokeh/Flamengo_xg_vs_xga_large.html";
            } else if (width > 800) {
                iframeElement.src = "/Assets/Bokeh/Flamengo_xg_vs_xga_mid.html";
            } else {
                iframeElement.src = "/Assets/Bokeh/Flamengo_xg_vs_xga_small.html";
            }
    }

    // Call the function when the page loads and when the window is resized
    window.onload = checkWindowWidth;
    window.onresize = checkWindowWidth;
</script>
