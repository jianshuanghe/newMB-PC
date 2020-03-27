/**
 *  供应热度榜
 **/
function  supplyHot() {
    jQuery.ajax({
        beforeSend: function(xhr) {
            xhr.setRequestHeader("Authorization", "Bearer eyJhbGciOiJIUzUxMiJ9.eyJyYW5kb21LZXkiOiJjejBtYmkiLCJzdWIiOiIxMzEyMTc5MjQ3MCIsImV4cCI6MTU4NTYyMzIyMywiaWF0IjoxNTg1MDE4NDIzfQ.li4LUMZm-hWglvo4PG_OlywqoBDqmmMmDs4vH08WtPgfcLqeUrB-Nkn8ngYsmkCKWQxLr1hRp644hCatbL183Q");
        },
        url : "http://zhaojie0001.mynatapp.cc/rest-rp/instPush/supplyHot",
        type : 'get',
        async: false,
        contentType : 'application/json;charset=UTF-8',
        success : function(data) {
            for(var i= 0;i<data.content.length;i++) {
                var html = "";
                html += "<div class='List-body-somil' onclick='instDetails(" + data.content[i].id + ")'>";
                html +="<div class='banner-erwei'><img src='./img/erweima.png' alt=''>";
                html +="<div class='home-erweima'>";
                html +="<div class='home-erwei'>手机端预览</div>";
                html +="<div class='home-erweima-img'>";
                html +="<img src='../../images/img/erweimakuang.png'>";
                html +="<div><img src='"+ data.content[i].purchaseQrimg +"'></div>";
                html +="</div>";
                html +="<div class='home-erweima-ti'>支持手机浏览器、微信小程序、百度小程序、支付宝小程序、头条小程序访问</div>";
                html +="<div class='home-erweima-look'>查看海报二维码</div>";
                html +="</div>";
                html +="</div>";
                html += "<div class='body-somil'>";
                html += "<div class='body-somil-tuwen'>";
                html += "<div class='somil-tuwen-tu'><img src='" + data.content[i].instLogo + "'></div>";
                html += "<div class='somil-tuwen-wen'>";
                html += "<div>" + data.content[i].instName+"</div>";
                if(data.content[i].moneyStr!=''){
                    html += "<div>"+ data.content[i].moneyStr + "</div>";
                }
                html += "</div>";
                html += "</div>";
                html += "<div class='body-somil-bot'>";
                html += "<div><img src='./img/Eye.png'>"+data.content[i].lookCount +"</div>";
                html += "<div><img src='./img/zan.png'>"+data.content[i].likeCount +"</div>";
                html += "<div><img src='./img/liuyan.png'>"+data.content[i].messageCount +"</div>";
                html += "<div class='body-somil-bot-xun'>立即询价</div>";
                html += "</div>";
                html += "</div>";
                html += "</div>";
                $(".List-body").append(html);
            }
            console.log(data);
        }
    });
}
/**
 *  采购热度榜
 **/
function  purchaseHot() {
    jQuery.ajax({
        beforeSend: function(xhr) {
            xhr.setRequestHeader("Authorization", "Bearer eyJhbGciOiJIUzUxMiJ9.eyJyYW5kb21LZXkiOiJjejBtYmkiLCJzdWIiOiIxMzEyMTc5MjQ3MCIsImV4cCI6MTU4NTYyMzIyMywiaWF0IjoxNTg1MDE4NDIzfQ.li4LUMZm-hWglvo4PG_OlywqoBDqmmMmDs4vH08WtPgfcLqeUrB-Nkn8ngYsmkCKWQxLr1hRp644hCatbL183Q");
        },
        url : "http://zhaojie0001.mynatapp.cc/rest-rp/instPush/purchaseHot",
        type : 'get',
        async: false,
        contentType : 'application/json;charset=UTF-8',
        success : function(data) {
            for(var i= 0;i<data.content.length;i++) {
                var html = "";
                if(data.content[i].purchaseImg==''){
                    html +="<div class='bodytwo-wenzi' onclick='purchaseDetail("+ data.content[i].id +")'>";
                    html +="<div class='banner-erwei'><img src='./img/erweima.png' alt=''>";
                    html +="<div class='home-erweima'>";
                    html +="<div class='home-erwei'>手机端预览</div>";
                    html +="<div class='home-erweima-img'>";
                    html +="<img src='../../images/img/erweimakuang.png'>";
                    html +="<div><img src='"+ data.content[i].purchaseQrimg +"'></div>";
                    html +="</div>";
                    html +="<div class='home-erweima-ti'>支持手机浏览器、微信小程序、百度小程序、支付宝小程序、头条小程序访问</div>";
                    html +="<div class='home-erweima-look'>查看海报二维码</div>";
                    html +="</div>";
                    html +="</div>";
                    html +="<div class='bodytwo-wenzi-box'>";
                    html +="<div>"+  data.content[i].purchaseName +"</div>";
                    html +="<div class='wenzi-box-fu'>"+data.content[i].contentInfo+"</div>";
                    html +="<div class='wenzi-box-but'>立即报价</div>";
                    html +="</div>";
                    html +="</div>";
                }else{
                    html += "<div class='bodytwo-About' onclick='purchaseDetail("+ data.content[i].id +")'>";
                    html +="<div class='banner-erwei'><img src='./img/erweima.png' alt=''>";
                    html +="<div class='home-erweima'>";
                    html +="<div class='home-erwei'>手机端预览</div>";
                    html +="<div class='home-erweima-img'>";
                    html +="<img src='../../images/img/erweimakuang.png'>";
                    html +="<div><img src='"+ data.content[i].purchaseQrimg +"'></div>";
                    html +="</div>";
                    html +="<div class='home-erweima-ti'>支持手机浏览器、微信小程序、百度小程序、支付宝小程序、头条小程序访问</div>";
                    html +="<div class='home-erweima-look'>查看海报二维码</div>";
                    html +="</div>";
                    html +="</div>";
                    html += "<div class='bodytwo-About-tu'>";
                    html += "<div class='About-tu-img'><img src='"+ data.content[i].purchaseImg +"' alt=''></div>";
                    html += "<div class='About-tu-zi'>";
                    html += "<div>" + data.content[i].purchaseName + "</div>";
                    html += "<div class='About-tu-zi-bao'>立即报价</div>";
                    html += "</div>";
                    html += "</div>";
                    html += "</div>";
                }
                $(".List-bodytwo").append(html);
            }
            console.log(data);
        }
    });
}