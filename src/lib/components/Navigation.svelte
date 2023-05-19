<aside>
    <nav>
        <ul>
            <li>
                <h2>Unlimiter</h2>
                <ul>
                    <li><a href="/home"><img src="/images/folder.svg" alt="icône de dossier">Home</a></li>
                    <li><a href="/unlimiter"><img src="/images/folder.svg" alt="icône de dossier">Unlimiter</a></li>
                </ul>
            </li>
            <li>
                <h2>3D Models</h2>
                <ul>
                    <li><a href="/blocks"><img src="/images/folder.svg" alt="icône de dossier">Default Blocks</a></li>
                    <li><a href="/skins"><img src="/images/folder.svg" alt="icône de dossier">Skins</a></li>
                    <li><a href="/united"><img src="/images/folder.svg" alt="icône de dossier">United</a></li>
                    <li><a href="/stadium"><img src="/images/folder.svg" alt="icône de dossier">Stadium</a></li>
                    <li><a href="/deco"><img src="/images/folder.svg" alt="icône de dossier">Deco</a></li>
                    <li><a href="/others"><img src="/images/folder.svg" alt="icône de dossier">Others</a></li>
                </ul>
            </li>
            <li>
                <h2>Textures</h2>
                <ul>
                    <li><a href="/textures"><img src="/images/folder.svg" alt="icône de dossier">Textures</a></li>
                </ul>
            </li>
            <li>
                <h2>Trackmania</h2>
                <ul>
                    <li><a href="/server"><img src="/images/folder.svg" alt="icône de dossier">Server</a></li>
                    <li><a href="/tracks"><img src="/images/folder.svg" alt="icône de dossier">Tracks</a></li>
                    <li><a href="/tools"><img src="/images/folder.svg" alt="icône de dossier">Tools</a></li>
                    <li><a href="/tm20"><img src="/images/folder.svg" alt="icône de dossier">TM20</a></li>
                    <li><a href="/canyon"><img src="/images/folder.svg" alt="icône de dossier">Canyon</a></li>
                </ul>
            </li>
            <li>
                <h2>Skins</h2>
                <ul>
                    <li><a href="/team"><img src="/images/folder.svg" alt="icône de dossier">Team</a></li>
                </ul>
            </li>
        </ul>
    </nav>
</aside>

<style lang="scss">
    aside{
      width: 180px;
      overflow-y: scroll;
    }

    nav{
      margin: 0 1.5rem;
      h2{
        color: var(--white-text);
        font-size: .9rem;
        margin-top: 2rem;
        margin-bottom: 1rem;
      }
      li{
        color: var(--white-text);
      }
      a{
        display: inline-block;
        width: 100%;
        padding: .5rem 0;
        img{
          padding-left: .5rem;
        }
      }
      ul li ul li{
        border-radius: 5px;
        font-size: .8rem;
        transition: all 200ms;
        &:hover{
          background: var(--hover-menu-bg);
        }
      }
      a{
        display: flex;
      }
    }

    img {
      width: 1rem;
      filter: invert(100%);
      margin-right: .5rem;
    }


</style>