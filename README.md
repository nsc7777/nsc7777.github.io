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
    
    <script src="https://dapi.kakao.com/v2/maps/sdk.js?appkey=f531c1f630564df9b868ad1cbecd9733"></script>
    
    <script>
        // 스크립트 로드 확인
        if (typeof kakao !== 'undefined') {
            var container = document.getElementById('map');
            var options = {
                center: new kakao.maps.LatLng(37.5665, 126.9780),
                level: 3
            };
            var map = new kakao.maps.Map(container, options);
            console.log('지도 로드 성공!');
        } else {
            console.error('카카오맵 API 로드 실패');
            alert('카카오맵을 불러올 수 없습니다. 개발자 도구(F12)에서 에러를 확인하세요.');
        }
    </script>
</body>
</html>
