jquery.inplaceForm is a collection of jQuery plugins that simplify inplace form
activities.

* jquery.inplaceListAdder *

inplaceListAdder is a plugin allowing for AJAX additions to lists like 
comments, todo items, etc. It has three modes: insert, append, and prepend.

Usage:

    $('#myform').inplaceListAdder('#mylist', options);

Options (and their defaults):

    {
        mode: 'insert', //insert, append, prepend        
        loadingImage: $.inplaceForm.defaultImage,
        iframe: false,  //submit form in an iframe?

        //callbacks
        submit: function(){},
        success: function(newItem){return true;},
        postsuccess: function(newItem){},
        error: function(errorDict){return true;},

        //selectors
        loadingSelector: '.loading',
        cancelSelector: '.cancel',
        errorSelectors:{} //key value pairs: { ErrorKey: '#selectorForError' }
    };

* jquery.inplaceListAdder *

inplaceListEditor is a plugin for editing list items (comments, etc.) in 
place.

* jquery.bindsaveForm *

bindsaveForm will bind ctrl+s to your forms.