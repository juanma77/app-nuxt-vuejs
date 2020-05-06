<template>
    <div>
        <h1 class="statement">Learn more about our new website</h1>
        <p class="bodytext">We grow the finest websites with our secret recipe.</p>
        <p class="bodytext">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas in 
            urna sed mauris consequat semper. Vestibulum faucibus id velit facilisis
            pharetra. Vivamus tincidunt orci eget metus pretium tristique. Nullam mi
            massa, interdum et sagittis in, pellentesque id metus. Praesent in 
            mattis purus, vitae auctor nisi. Maecenas ut orci nec urna vestibulum
            laoreet. Phasellus lacinia iaculis imperdiet. Nullam tincidunt velit
            eu tortor varius scelerisque. Nullam placerat ligula tincidunt mi
            placerat blandit.
            Interdum et malesuada fames ac ante ipsum primis in faucibus. Maecenas sodales
            finibus diam, a aliquet sapien. Nam molestie eros non tincidunt facilisis.
            Praesent facilisis massa a lorem commodo, a ultricies arcu vehicula. Curabitur a
            tincidunt magna. Maecenas porta sodales turpis id tempus. Etiam fringilla
            tincidunt ullamcorper. Phasellus quis dolor dignissim, tincidunt dolor et,
            viverra neque. Praesent at tellus turpis. Integer nec aliquet est, ut ultricies
            ex. Sed purus ex, pretium ut facilisis quis, accumsan eu elit. Nullam ac egestas
            metus, non viverra libero. Integer a turpis diam. Duis ullamcorper eleifend est
            id ullamcorper.
        </p>
        <nuxt-link to="/" class="callToAction">Go Back</nuxt-link>
    </div>
</template>

<script>
export default {
    /* Sobreescribimos los valores por defecto del head
    para asegurarnos que tenemos una buena descripción y palabras
    claves incrustadas como metadatos.
    Cuaqluier valor puesto aquí sobreescribirá cualquier valor en 
    el head escrito en el archivo nuxt.config.js*/
    head(){
        return {
            title: `About our websites`,
            meta: [
                { hid: 'description', name:'description', content: 'WebsiteCo provides the finest in modern websites' },
                { name: 'keywords', content: 'websiteCo, websites, website design' }
            ]
        }
    }
}
</script>  