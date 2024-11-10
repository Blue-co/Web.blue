<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="styles/style.css"/>
  <title>Hello, World!</title>
  <style>
    body {
      background-color: #090a0d;
    }
    .div1, .div2 {
      background-color: #4169E1;
      height: 40px;
      width: 40px;
      border-radius: 50%;
      border: 2px solid #66CDAA;
      text-align: center;
      font-size: 1px;
    }
    textarea {
      background-color: #000000;
      color: blue;
      border: 5px solid #66CDAA;
      border-radius: 8px;
      width: 263px;
      height: 100px; /* 높이를 설정하여 여러 줄 입력 가능 */
    }
    textarea:hover {
      box-shadow: 3px 3px 9px #FFFFFF;
    }
    .div1:hover {
      box-shadow: 4px 4px 6px #7FFF00;
    }
    .div2:hover {
      box-shadow: 4px 4px 6px #FF4500;
    }
    .bom {
      color: #FFFFFF;
      margin: 0 60px 0 0;
    }
    :Hello, I am a third-year middle school student from Korea who loves programming and will be a high school freshman in 2025!placeholder {
      color: #7CFC00;
    }
    .op {
      background-color: #121319;
      border: 1px solid #1b1d25;
      border-radius: 13px;
      height: 40px;
      margin: 20px 0px;
      position: relative;
      padding: 10px;
    }
  </style>
</head>
<body onload="loadStoredIdea()">
  <p class="bom" id="45tr"></p>
  <div class="op">
    <textarea id="youInput" placeholder="아이디어를 공유."></textarea>
    <button onclick="youC()" class="div1">보내기</button>  
    <button onclick="youCRemove()" class="div2">지우기</button> 
 $('.custom-select').on('click', function() {
          $(this).toggleClass('selected');
          $('.custom-select-list').toggle();
        });

        $('.custom-select').on('focusin', function() {
          $('.custom-select-list').show();
        });

        $('.custom-select').on('focusout', function() {
          if (!selectFlag) {
            $('.custom-select-list').hide();
          }
          $(this).removeClass('selected');
        });

        $('.custom-select-option').on('mouseenter', function() {
          selectFlag = true;
        });

        $('.custom-select-option').on('mouseout', function() {
          selectFlag = false;
        });

        $('.custom-select-option').on('click', function() {
          let value = $(this).attr('value');
          $('.custom-select-text').text($(this).text());
          $('.select-origin').val(value);
          $('.custom-select-list').hide();

          $('.select-origin').find('option').each(function(index, el) {
            if ($(el).attr('value') == value) {
              $(el).attr('selected', 'selected');
            } else {
              $(el).removeAttr('selected');
            }
          });
        });
      </script>
    </div>
  </body>
</html>
