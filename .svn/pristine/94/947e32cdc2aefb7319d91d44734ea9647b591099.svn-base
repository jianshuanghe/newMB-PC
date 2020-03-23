<script type="text/javascript">
    $.fn.toggle = function( fn ) {
        // Save reference to arguments for access in closure
        var args = arguments,
                guid = fn.guid || jQuery.guid++,
                i = 0,
                toggler = function( event ) {
                    // Figure out which function to execute
                    var lastToggle = ( jQuery._data( this, "lastToggle" + fn.guid ) || 0 ) % i;
                    jQuery._data( this, "lastToggle" + fn.guid, lastToggle + 1 );
 
                    // Make sure that clicks stop
                    event.preventDefault();
 
                    // and execute the function
                    return args[ lastToggle ].apply( this, arguments ) || false;
                };
 
        // link all the functions, so any of them can unbind this click handler
        toggler.guid = guid;
        while ( i < args.length ) {
            args[ i++ ].guid = guid;
        }
 
        return this.click( toggler );
    }
</script>
    



<!-- jQuery的toggle()方法应该是在鼠标点击后才会触发，现在的问题是在ready加载后就自动触发了，怎么回事呢？

答案是jQuery的版本问题，在1.9以后的版本toggle()就存在这个问题，用之前的版本就正常了。​

如果你非常喜欢这个功能，有2个办法，一个办法是jquery官网提供的一个版本升级文件。http://blog.jquery.com/2013/05/08/jquery-migrate-1-2-1-released/

另外一个办法是笨办法，就是把原来的那块代码拿出来，写成一个插件。 -->