1. Go to [here (mitmproxy website)](https://docs.mitmproxy.org/stable/overview/installation/), and download the Linux binaries.


2. Extract them to your home folder.


3. Now, this is an important step. You need two browsers. One, your main browser, that you use for everything and is where you will use the mitmweb interface. The second, the well, secondary browser. You will route this through mitmproxy and exculsively use that browser for mitmproxy related things. Go get a browser for this. In this guide, I will be using Waterfox as my main browser and Firefox as my secondary, although the two in this case are interchangable.


4. Make sure the `mitmweb` executable has the proper permissions to run. You may need to use `chmod`.


5. Run it from your command line with the command `./mitmweb --listen-port 8082`. This will host the interface in your browser, which will now open, and it will begin listening on `localhost:8082`. However, the second browser must be configured to route through that.


6. In this case the secondary browser is firefox/waterfox, so I will list instructions for that. Go to firefox, go to settings, and open your proxy settings. Select "Manual proxy configuration", and in the "Http Proxy" field type `localhost`, and in the port type `8082`. Then, check the "also use this proxy for https" box and hit OK.


7. In your secondary browser, visit the "magic domain" `mitm.it`. There you will see a list of certificates. In this case, download the Firefox one (will work for firefox and waterfox).


8. Go back to your secondary browser settings, and search for "certificates", then click "View Certificates". You should see an "Import" button.


9. Click view imports and import the file downloaded from `mitm.it` with all permissions boxes checked, and hit OK when done.


10. Go to your `mitmweb` interface in your primary browser. Search something in firefox, and you should now be able to see and modify and replay traffic!


11. You can restart mitmweb once you close it or restart it with the command used the first time to start it. Your secondary browser may show a connection error if you try to use it and mitmproxy is not running, that is normal and makes sense, because it can't find mitmproxy to route through.


