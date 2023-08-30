function GeneratePageNumbers() {
  
  let slides = SlidesApp.getActivePresentation().getSlides();
  let slidesLen = slides.length;
  let strSlidesLen = slidesLen.toString();

  for( let i = 1; i < slidesLen; i++){
    let pageNumber = slides[i].getPlaceholder(SlidesApp.PlaceholderType.SLIDE_NUMBER).asShape();
    let strPageNum = pageNumber.getText();
    strPageNum.setText((i+1).toString());
    strPageNum.appendText('/');
    strPageNum.appendText(strSlidesLen);
    
  }
}
