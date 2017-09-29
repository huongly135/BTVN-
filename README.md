<html
data-sbro-popup-lock="true" data-sbro-ads-lock="true" data-sbro-deals-lock="true" data-sbro-extensions-lock="true"><head><style></style></head><body>
<div style="width:100%;height:120px;">
<div style="background-color:#06FA2E;width:170px;height:80px;margin:20px;padding-top:20px;color:#ffffff;font-weight:bold;font-size:18px;float:left;text-align:center;" onmouseover="this.innerHTML='I am KÏNG Corvuš š '" onmouseout="this.innerHTML='HELLO'">Xin chào</div>
<div style="background-color:#7F8AF4;width:170px;height:80px;margin:20px;padding-top:20px;color:#ffffff;font-weight:bold;font-size:18px;float:left;text-align:center;" onclick="clickMeEvent(this)">Please click me</div>
  </div>
  <script type="application/javascript">
function clickMeEvent(obj) {
  if (obj.innerHTML == "Please click me") {
    obj.innerHTML = "Please click me<br>Again";
    return;
  }
  if (obj.innerHTML == "Please click me<br>Again") {
    obj.innerHTML = "WELCOME TO LEAGUE OF LEGEND";  
    return; 
  }
  if (obj.innerHTML == "WELCOME TO LEAGUE OF LEAGEND") {
  obj.innerHTML = "LOL";  
    return; 
  }
  if (obj.innerHTML == "LOL") {
    obj.style.display = "none";
    return;
  }
}
</script>
<br><h3>TEST 1</h3>
<h2 onclick="this.innerHTML='Hello my friend'">Please click here</h2>
<p id="demo"></p> 
<div onmousedown="mDown(this)" onmouseup="mUp(this)" style="background-color:#E51DD4;width:90px;height:90px;padding:40px;">
Bạn có thể ấn thử</div>
<script>
function mDown(obj) {
    obj.style.backgroundColor = "#E2E51D";
    obj.innerHTML = "What do you see ?";
}

function mUp(obj) {
    obj.style.backgroundColor="#08F4F0";
    obj.innerHTML="Please tell me what do you see!";
}
function myFunction() {
    document.getElementById("demo").innerHTML = "";
}

document.getElementById("myBtn").onclick = function(){displayDate()};

function displayDate() {
    document.getElementById("demo").innerHTML = Date();
}
</script>
<span onmouseover="this.style.color='blue'">Hãy di chuột vào và tận hưởng sự khác biệt</span>

 
</body><script>function patch() {

    window._open = window.open;
    document._createElement = document.createElement;
    document._createEvent = document.createEvent;
    window._parent = (window.location != window.parent.location) ? document.referrer: document.location;

    function getParent(el, selector) {
        var parent = el.parentNode;
        if (parent == document) {
            return null;
        }
        if (parent.matches(selector)) {
            return parent;
        } else {
            return getParent(parent, selector);
        }
    }

    function blockWindow(args) {
        var target;
        if (window.event) {
            target = window.event.target.tagName.toLowerCase() == 'a' ?
                window.event.target : getParent(window.event.target, 'a');
        }
        parent.postMessage({
            type: "safeBlock",
            url: args && args.length > 0 ? args[0] : '',
            args: args ? Array.from(args) : null,
            href: target ? target.href : null
        }, window._parent);
    }

    window.open = function() {
        blockWindow(arguments);
    };

    dispatchEvent = function(element) {
        return function(event) {
            if (event.type == "click") {
                blockWindow([element.getAttribute('href')]);
            }
        }
    };

    document.createElement = function() {
        var element = document._createElement.apply(document, arguments);
        if (arguments[0].toLowerCase() == 'a') {
            element.dispatchEvent = dispatchEvent(element);
        }
        return element;
    };

    // Process saved popup.
    var html = document.querySelector('html'),
        key = 'data-sbro-popup-current',
        url = html.getAttribute(key);
    if (url) {
        blockWindow([url]);
    }

}; patch();</script></html>
