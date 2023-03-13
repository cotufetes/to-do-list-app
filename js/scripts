function newItem(){

    //1. Adds new item to the list
    let li = $('<li></li>');
    let inputValue = $("#input").val();
    li.append(inputValue);

    if (inputValue === '') {
        alert("You must write something!");
    } else {
        $('#list').append(li);
    }

    //2. Crosses out an item
    li.on("dblclick", function(){
        li.toggleClass("strike");
    });

    //3. Adds the delete button "X"
    let crossOutButton = $('<crossOutButton></crossOutButton>');
    crossOutButton.append(document.createTextNode('X'));
    li.append(crossOutButton);
  
    crossOutButton.on("click", function(){
        li.addClass("delete");
    });

    // 4. Allows reordering of list items 
    $('#list').sortable();

}