<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gardenia</title>
</head>
<body>
    <!-- JavaScript to load the chatbot asynchronously -->
    <script>
        function loadChatbotScript() {
            var script = document.createElement('script');
            script.src = 'https://cdn.botpress.cloud/webchat/v1/inject.js';
            script.async = true;
            document.body.appendChild(script);

            script.onload = function () {
                window.botpressWebChat.init({
                    "botId": "c62a2450-ad70-492f-878a-c2a9732a6458",
                    "clientId": "c62a2450-ad70-492f-878a-c2a9732a6458",
                    "hostUrl": "https://cdn.botpress.cloud/webchat/v0",
                    "messagingUrl": "https://messaging.botpress.cloud",
                    "botName": "Gardenia",
                    "avatarUrl": "https://i.postimg.cc/NMYxmYRP/image502-1695792437594.jpg",
                    "containerWidth": "100%25",
                    "layoutWidth": "100%25",
                    "composerPlaceholder": "Start typing here",
                    "botConversationDescription": "Your Property Partner",
                    "hideWidget": true,
                    "stylesheet": "https://webchat-styler-css.botpress.app/prod/code/5ce2b2c8-4482-424a-8e12-ad6bba19692c/v62394/style.css",
                    "disableAnimations": true,
                    "lazySocket": false,
                    "useSessionStorage": true,
                    "frontendVersion": "v1",
                    "enableConversationDeletion": true
                });
                window.botpressWebChat.onEvent(function () {
                    window.botpressWebChat.sendEvent({ type: 'show' });
                }, ['LIFECYCLE.LOADED']);
            };
        }

        // Call the function to load the chatbot script
        loadChatbotScript();
    </script>
</body>
</html>
