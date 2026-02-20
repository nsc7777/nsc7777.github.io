<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>카카오맵</title>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        html, body {
            width: 100%;
            height: 100%;
        }
        #map {
            width: 100%;
            height: 100%;
        }
    </style>
</head>
<body>
    <div id="map"></div>
    
    <!-- 1. 여기에 발급받은 키 입력 -->
    <script src="//dapi.kakao.com/v2/maps/sdk.js?appkey=f531c1f630564df9b868ad1cbecd9733"></script>
    
    <script>
        // 2. 이 부분은 그대로 사용
        var container = document.getElementById('map');
        var options = {
            center: new kakao.maps.LatLng(37.5665, 126.9780),
            level: 3
        };
        var map = new kakao.maps.Map(container, options);
    </script>
</body>
</html>
