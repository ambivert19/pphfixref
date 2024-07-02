<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">

<head>
    <meta name="generator" content="HTML Tidy, see www.w3.org" />
    <meta http-equiv="Content-Type" content="text/html;charset=UTF-8" />
    <meta http-equiv="CACHE-CONTROL" content="NO-CACHE" />
    <meta http-equiv="PRAGMA" content="NO-CACHE" />
    <meta http-equiv="EXPIRES" content="-1" />
    <meta name="ROBOTS" content="NONE" />

    <meta charset="utf-8">

    <link type="text/css" href="/SimpleTextQuery.css" rel="stylesheet" media="screen" />
    <script type="text/javascript" src="/SimpleTextQuery.js"></script>

    <script type="text/javascript">
        // Function to handle form submission
        function handleFormSubmit(event) {
            event.preventDefault();
            
            var freetext = document.getElementById('freetext').value;

            // Validate input
            if (freetext.trim() === "") {
                alert("Please enter some text in the box.");
                return;
            }

            // Prepare data for submission
            var formData = new FormData(event.target);

            // Simulate an asynchronous operation (e.g., sending data to a server)
            // For demonstration, we're using a timeout to mimic a server request
            setTimeout(() => {
                alert("Form submitted successfully!");
                console.log("Submitted data:", Object.fromEntries(formData.entries()));
            }, 1000);
        }

        // Add event listener to the form
        document.addEventListener('DOMContentLoaded', (event) => {
            document.querySelector('form[name="freeTextQuery"]').addEventListener('submit', handleFormSubmit);
        });
    </script>

    <!-- Matomo -->
    <script type="text/javascript">
        var _paq = window._paq || [];
        _paq.push(["setDocumentTitle", document.domain + "/" + document.title]);
        _paq.push(["setCookieDomain", "*.apps.crossref.org"]);
        _paq.push(['trackPageView']);
        _paq.push(['enableLinkTracking']);
        (function() {
            var u = "https://crossref.matomo.cloud/";
            _paq.push(['setTrackerUrl', u + 'matomo.php']);
            _paq.push(['setSiteId', '9']);
            var d = document, g = d.createElement('script'), s = d.getElementsByTagName('script')[0];
            g.type = 'text/javascript'; g.async = true; g.defer = true; g.src = u + 'matomo.js'; s.parentNode.insertBefore(g, s);
        })();
    </script>
    <noscript><p><img src="https://crossref.matomo.cloud/matomo.php?idsite=9&rec=1" style="border:0;" alt="" /></p></noscript>
    <!-- End Matomo Code -->

    <title>Simple Text Query</title>
</head>

<body style="text-align: center;margin: 0px;">
    <div class='debug-eyeline'></div>
    <div id="back-to-site" style="background: #ffc72c; height: auto; line-height: 36px; color: #000; text-align: center; padding: 3px 0; color: #000;font-family: HelveticaNeueETW01-55Rg, 'Helvetica Neue', Helvetica, Arial, sans-serif;
font-size: 14px;direction: ltr;">
        &#8592; <a style="text-decoration: underline;transition: color 0.1s linear;cursor: pointer;background: transparent;line-height: 36px;text-align: center;font-family: HelveticaNeueETW01-55Rg, 'Helvetica Neue', Helvetica, Arial, sans-serif;font-size: 14px;direction: ltr;" href="https://www.crossref.org">Back to the main Crossref website</a>
    </div>

    <header class="d-header" style="left: 0; z-index: 1000; padding-top: 3px; height: 100px; width: 100%; position: absolute; top: 42; background-color: #fff; 
         box-shadow: 0 2px 4px -1px rgba(0,0,0,0.25);margin-bottom: 15px;">
        <div class="wrap" style="max-width: 1110px;margin-right: auto;margin-left: auto;padding: 0 8px;font-family: HelveticaNeueETW01-55Rg, 'Helvetica Neue', Helvetica, Arial, sans-serif;
font-size: 14px;color: #222;line-height: 19px;direction: ltr;">
            <div class="contents" style="margin: 8px 0;position: relative;">
                <div class="row">
                    <div class="title" style="float: left;">
                        <a href="https://www.crossref.org">
                            <img src="https://assets.crossref.org/logo/crossref-logo-landscape-200.svg" width="200" height="68" alt="Crossref" id="site-logo" style="max-height: 40px;vertical-align: middle;">
                        </a>
                    </div>
                    <div class="title" style="float: right;">
                        <a href="https://www.crossref.org/blog/a-simpler-text-query-form/">
                            <img src="/images/blog-ad-stq-2019.png" width="220" height="90" alt="Crossref ad" id="site-logo" style="max-height: 80px;vertical-align: top; display: inline !important; visibility: visible !important; opacity: 1 !important;">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <div id="main-outlet" class="wrap" style="padding-top: 82px;max-width: 1110px;margin-right: auto;margin-left: auto;padding: 0 8px;color: #222;line-height: 19px;direction: ltr;">
        <div id="mainContent2" style="padding-top: 103px;">
            <div>
                <form enctype="application/x-www-form-urlencoded" method="POST" name="freeTextQuery" accept-charset="UTF-8">
                    <font style="font-size: 16px">
                        <table>
                            <tr valign="top">
                                <td valign="top">
                                    <table width="95%" height="100%" border="0" cellspacing="0" cellpadding="0">
                                        <tr height="100%" valign="top">
                                            <td align="left" valign="top"><img src="https://wwwold.crossref.org/images/spacer.gif" alt="" height="1" width="1" border="0" /></td>
                                            <td height="100%" align="left" valign="top">
                                                <input id="command" type="hidden" name="command" value="" /><br />
                                                <                                                <textarea id="freetext" name="freetext" rows="20" cols="100" style="font-size: 16px; width: 100%;"></textarea><br />
                                                <input type="submit" value="Submit" style="font-size: 16px;"/>
                                            </td>
                                        </tr>
                                    </table>
                                </td>
                            </tr>
                        </table>
                    </font>
                </form>
            </div>
        </div>
    </div>

    <footer class="d-footer" style="background-color: #f8f8f8; padding: 20px 0; margin-top: 20px;">
        <div class="wrap" style="max-width: 1110px; margin-right: auto; margin-left: auto; padding: 0 8px;">
            <div class="footer-contents" style="font-family: HelveticaNeueETW01-55Rg, 'Helvetica Neue', Helvetica, Arial, sans-serif; font-size: 14px; color: #222; line-height: 19px;">
                <p>&copy; 2024 Crossref. All rights reserved.</p>
                <p><a href="https://www.crossref.org/privacy/">Privacy Policy</a> | <a href="https://www.crossref.org/terms/">Terms & Conditions</a></p>
            </div>
        </div>
    </footer>
</body>

</html>

