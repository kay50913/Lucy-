# Lucy-html
<!DOCTYPE html>
<html>
<head>
    <title>聖誕節驚喜</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
        }
        
        .tree {
            font-size: 50px;
            cursor: pointer;
        }
        
        .tree:hover {
            color: red;
        }
        
        #video-frame {
            display: none;
        }
        
        #message {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>聖誕節驚喜アプリ</h1>
    <div class="tree" onclick="showVideo()">&#127876;</div>
    <div id="video-frame">
        <iframe width="560" height="315" src="[https://www.youtube.com/embed/?listType=user_uploads&list=taiwanwondering](https://youtube.com/playlist?list=PLj_rp8v_tcGAseXSbQjlj5XajxKA8d4_3&si=QADcDK9wfZuUTcqY)" allowfullscreen></iframe>
    </div>
    <div id="message">
        <input type="text" id="message-box" placeholder="佳節愉快、聖誕節重要意義のメッセージを入力してください" oninput="updateMessage()" />
    </div>

    <script>
        function showVideo() {
            document.getElementById("video-frame").style.display = "block";
        }

        function updateMessage() {
            var message = document.getElementById("message-box").value;
            document.getElementById("message").innerHTML = message;
        }
    </script>
</body>
</html>
