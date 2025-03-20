Kort refleksion:

    Reflekter kort men fagligt over din løsning med henblik på udfordringerne og successerne ved opgaven.

    En af de største udfordringer i denne opgave var at oversætte Figma-designet præcist til kode. Der var flere detaljer i designet, som krævede præcise CSS-justeringer, især ved brug af Grid for at opnå det ønskede layout. En stor succes var brug af subgrid. Dette har været et helt ny GENIAL måde at kunne kode på. Ved subgrid kan man genbruge de tideligere koder, og derved gøre sit css mere vedligelsesvenligt.

    Fremhæv specifikke kodestumper, der illustrerer brugen af forskellige teknikker og principper (gerne fra undervisningen).

    Det nye vi har lært er hvordan vi kan styre vores layout ved brug af grid og subgrid. Dette er en super smart og let med hvorpå man får en mere fleksibel, responsiv og centreret sideindholdsstuktur:
    Jeg har brugt den til mit blandt andet min main.
    Den gør sektionerne ensartede, sikrer at indholdet altid er centreret, og forenkler min styling.

    main {
    > section {
        grid-column: full;
        display: grid;
        grid-template-columns: subgrid;
        padding-block: 4rem;

        > * {
            grid-column: content;
        }
    }

}

    Forklar, hvordan du har organiseret din CSS; hvornår er det globalt, og hvornår er det komponent-specifikt.

    Jeg har organiseret mit CSS ved brug af bland andet global.css. Dette har jeg brugt til blandt andet mine farver, font-family, line-height, font-weight samt andre elementer som gå igen på de andre sider.
    Ved at lave de gentagnene elementer og css i en samlet global fil, sørger jeg for at siderne er identiske.
    Jeg har sagtens kunne optimere her, da flere at mine sider indeholder gentangene elementer.
