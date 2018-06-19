$(function formatCBL() {

    var contentBylabel = $(".content-by-label");
    var anchors = contentBylabel.find("div>a");
    // Remove label's existing parent elements and wrap in h2's
    anchors.unwrap();
    anchors.wrap("<h2 class='wiki-content'></h2>");
    
    // Iterate through each li in the default output, remove 
    // superfluous HTML
    contentBylabel.find("li").each(function format() {
        var me = $(this);
        me.find("div").first().remove();
        var outerSpan = me.find("span:first")
        // split on this long dash so we can get rid of it
        text = outerSpan.html().split("—");
        me.find("span").html(text[1]);
    });

    contentBylabel.find("p").unwrap();

});
