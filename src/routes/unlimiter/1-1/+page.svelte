<script>
    import Unlimiter from "$lib/components/Unlimiter.svelte";

    let unlimiterDetails = {
        version: '1.1',
        background: 'url("/images/unlimiter1-3.jpg")',
        documentation: [
            {
                icon: '/images/drive.svg',
                alt: 'Alternative',
                name: 'Gdoc',
                description: 'TMInfinity (Unlimiter 1.1) Documentation',
                link: '/'
            },
            {
                icon: '/images/github.svg',
                alt: 'Alternative',
                name: 'Github',
                description: 'Blender Plugin 3.1+',
                link: '/'
            },
            {
                icon: '/images/material.svg',
                alt: 'Alternative',
                name: 'Material',
                description: 'Material documentation',
                link: '/'
            },
        ],
        scripts: [
            {
                name: 'Script 1',
                description: 'Description 1',
                path: '/',
            },
            {
                name: 'Script 2',
                description: 'Description 2',
                path: '/',
            },
            {
                name: 'Script 3',
                description: 'Description 3',
                path: '/',
            },
            {
                name: 'Script 4',
                description: 'Description 4',
                path: '/',
            },
            {
                name: 'Script 5',
                description: 'Description 5',
                path: '/',
            },
            {
                name: 'Script 6',
                description: 'Description 6',
                path: '/',
            },
        ]
    }
</script>

<Unlimiter {unlimiterDetails}/>