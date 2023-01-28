<script>
    export let value;
    let link=true;
    function handleBackClick(){
        if(link){
            window.history.back();
        }
        else{
            return false;
        }
    }
    if(!value){
        value="home";
        link=false
    }
</script>
<button on:click={handleBackClick}><a href="/" rel="history"><span style="color: #858585; text-decoration:inherit;"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#858585" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="inline feather feather-arrow-left"><line x1="19" y1="12" x2="5" y2="12"></line><polyline points="12 19 5 12 12 5"></polyline></svg>
     {value}</span></a></button><br>