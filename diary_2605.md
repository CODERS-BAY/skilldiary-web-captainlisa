# Diary 26.05.2020

* a session is a protocol that saves information and can send it between different pages.
* 
* you can load modals as soon as the page loads with this code:
```javascript
    <script 
        type="text/javascript">
        $(window).on('load',function(){
            $('#loginModal').modal('show');
        });
    </script>
```