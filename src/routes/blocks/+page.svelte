<script lang="ts">
    import BlockList from "$lib/components/BlockList.svelte";

    const elements = [
        {
            name: 'EightByEight',
            description: 'Description',
            folders: [
                {
                    img: '/images/folder.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Bay',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Bay',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Bay',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Stadium',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Stadium',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Stadium',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
        {
            name: 'Stadium',
            description: 'Description',
            folders: [
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230379513-16801bac-53fd-4202-a8b4-32f9516fda0d.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
                {
                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                    subfolders: [
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230388623-0c77b6d6-cec3-4d4a-b5af-2dd64ad40d49.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        },
                        {
                            img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                            items: [
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                                {
                                    img: 'https://user-images.githubusercontent.com/47508526/230381090-09b1b53a-9930-4e19-acf3-7404225ccc01.png',
                                    path: '/'
                                },
                            ]
                        }
                    ]
                },
            ]
        },
    ]
</script>

<BlockList {elements} />

