<script>
    let { content='Nothing', contentColor="white", btnBgColor='#c06422', btnBgHoverColor='#369392', borderWidth=2 } = $props();
</script>
<button 
    style="background-color: {btnBgColor}; border-color: {btnBgColor}; border-width: {borderWidth}px;"
    class="py-2 px-4 rounded-xl border transition-all duration-150"
    onmouseenter={(e) => {
        e.currentTarget.style.backgroundColor = btnBgHoverColor;
        e.currentTarget.style.borderColor = btnBgHoverColor;
    }}
    onmouseleave={(e) => {
        e.currentTarget.style.backgroundColor = btnBgColor;
        e.currentTarget.style.borderColor = btnBgColor;
    }}
>
    <p class="font-bold text-lg" style="color: {contentColor};">
        {content}
    </p>
</button>