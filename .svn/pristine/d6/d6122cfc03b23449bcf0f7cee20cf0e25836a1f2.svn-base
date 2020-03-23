function downloadImage(path,imgName) {
    var _OBJECT_URL;
    var request = new XMLHttpRequest();
    request.addEventListener('readystatechange', function (e) {
        if (request.readyState == 4) {
            _OBJECT_URL = URL.createObjectURL(request.response);
            var $a = $("<a></a>").attr("href", _OBJECT_URL).attr("download", imgName);
            $a[0].click();
        }
    });
    request.responseType = 'blob';
    request.open('get', path);
    request.send();
}
export { 
    downloadImage
};