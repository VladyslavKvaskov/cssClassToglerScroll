class cssClassTogglerScroll{
  constructor(element, cssClass){
    let elementBounding;
    let elementHeight;
    let windowHeight;
    windowHeight = window.innerHeight;
    const target = element.parentNode === document.body ? window : element.parentNode;
    let targetHeight = element.parentNode === document.body ? window.innerHeight : element.offsetHeight;
    target.addEventListener('scroll', function(){
      elementBounding = {
        top:element.getBoundingClientRect().top,
        bottom:element.getBoundingClientRect().bottom
      };

      elementHeight = element.offsetHeight;
      if(elementBounding.top < targetHeight - (elementHeight / 10) && elementBounding.bottom > elementHeight / 10){
        element.classList.add(cssClass);
      }
      else
        element.classList.remove(cssClass);
    });

      elementBounding = {top:element.getBoundingClientRect().top, bottom:element.getBoundingClientRect().bottom};
      elementHeight = element.offsetHeight;
      if(elementBounding.top < targetHeight - (elementHeight / 10) && elementBounding.bottom > elementHeight / 10){
        element.classList.add(cssClass);
      }
      else
        element.classList.remove(cssClass);
  }
}
