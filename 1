
//range slider
var $element = $('input[type="range"]');

$element
  .rangeslider({
    polyfill: false,
    onInit: function() {
      var $handle = $('.rangeslider__handle', this.$range);
      updateHandle($handle[0], this.value);
    }
  })
  .on('input', function(e) {
    var $handle = $('.rangeslider__handle', e.target.nextSibling);
    updateHandle($handle[0], this.value);
  });

function updateHandle(el, val) {
  el.textContent = val;
}

//calculator

$(document).ready(function() {
    //calculate values automatically 
    sum();
    $("#ram-total, #ram-reserved, #ram-buffer, #process-size").on("keydown keyup change", function() {
        sum();
    });
  generateConfigCopy();

  $("buttonCopy").click(function(){
    copyClipboard
  });

});

function sum() {
      //inputs
      var ramtotal = document.getElementById('ram-total').value;
      var ramreserved = document.getElementById('ram-reserved').value;
      var rambuffer = document.getElementById('ram-buffer').value;
      var processsize = document.getElementById('process-size').value;

      

      var buffer = 1 - (rambuffer / 100) ;

      //[Total Available RAM] – [Reserved RAM] – [10% buffer] = [Available RAM for PHP]
      var availableram = Math.round(((ramtotal - ramreserved) * buffer) * 10) / 10;
      var availablerammb = Math.round(availableram * 1024);

      // [Average Process Size] / [Available RAM for PHP]= [max_children]
      var maxchildren =  Math.floor(availablerammb / processsize);
      var startservers = Math.floor(maxchildren * 0.25);
      var minspare = Math.floor(maxchildren * 0.25);
      var maxspare = Math.floor(maxchildren * 0.75);


        if (!isNaN(availableram)) {
              //Outputs
              //document.getElementById('ram-buffer-percent').value = buffer;
              document.getElementById('ram-available').value = availableram;
              document.getElementById('ram-available-mb').value = Math.round(availableram * 1024);
              document.getElementById('max-children').value = maxchildren;
              document.getElementById('start-servers').value = startservers;
              document.getElementById('min-spare').value = minspare;
              document.getElementById('max-spare').value = maxspare;
            }
          }

function generateConfigCopy (){
document.getElementById('copyPasteArea').value = 'pm.max_children = ' + document.getElementById('max-children').value +'\n'
              + 'pm.start_servers = ' + document.getElementById('start-servers').value +'\n'
              + 'pm.min_spare_servers = ' + document.getElementById('min-spare').value +'\n'
              + 'pm.max_spare_servers = ' + document.getElementById('max-spare').value;

}

function copyClipboard (){
  var text = document.getElementById('copyPasteArea');
  text.select();
  document.execCommand('copy');
  alert('copied to clipboard successfully.');
}

