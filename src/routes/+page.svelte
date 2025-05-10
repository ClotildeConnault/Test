<script lang="ts">
    import Card from "$lib/fragment/Card/Card.svelte";
    import Button from "$lib/ui/Buttons/Button.svelte";

    let myState = $state(12);
    let myDerived = $derived(myState * 2);
    let color = "#8fcc9f";
</script>

<!-- <Button>{@render mySnippet(myDerived)}</Button>
<button onclick={() => myState++}>Click</button> -->

<div class="relative h-96 w-full mb-10 flex items-start">
    <div
        class="absolute top-0 left-0 h-full w-full bg-[url('/BG2.png')] bg-cover bg-center -z-10"
    ></div>
    <div class="absolute top-0 left-0 h-full w-full bg-black/20 -z-10"></div>

    <div class="select-none flex flex-col ml-[15vw] mt-32 items-center">
        <h1 class="relative text-white text-4xl">
            <img
                class="absolute h-40 -left-44 -translate-y-12"
                src="/logo3.png"
                alt="logo"
            />
            Église Protestante Évangélique de Liège
        </h1>
        <h2 class="text-white text-2xl">Culte tous les dimanches à 10h</h2>
        <div class="flex items-center gap-2 mt-8">
            <Button route="/presentation">Qui sommes-nous ?</Button>
            <Button route="/contact">Nous rencontrer</Button>
        </div>
    </div>
</div>

<div class="flex-1 bg-white p-4 space-y-4">
    <div class="flex flex-row items-center justify-center mr-10 ml-10 gap-10">
        <Card background="bible.jpg">Études Bibliques</Card>
        <Card background="prayer.jpg">Rencontres de prière</Card>
        <Card background="femmes.jpg">Rencontres pour les femmes</Card>
    </div>
    <div class="flex flex-row items-center justify-center mr-10 ml-10 gap-10">
        <Card background="enfants.jpg">Activités pour les enfants</Card>
        <Card {color} background="ados.jpg">Activités pour les ados</Card>
        <Card background="flags.png"
            >Rencontres en espagnol, roumain, arabe</Card
        >
    </div>
    <div class="flex flex-row gap-3">
        <!-- <Card>
                <p>Culte tous les dimanches à 10h</p>
                <p>Des assemblées partenaires se réunissent dans le local pour des réunions en roumain et en arabe.</p>
            </Card>
            <Card>
                <p>N’hésitez pas à nous contacter pour toutes ces activités. Nous sommes aussi disponibles pour vous rencontrer en toute simplicité si vous avez une question par rapport à la foi ou quoi que ce soit d’autre, nous sommes à l’écoute.</p>
                <p>Martin Bräker - 0471 / 74 03 20</p>
                <p>martin.braker@aepeb.be</p>
            </Card> -->
    </div>

    <!-- <p>Nous sommes une communauté de Chrétiens Protestants Évangéliques.</p>
        <p>
            Notre identité ? C'est celle d'individus pécheurs pardonnés et
            renouvelés par la grâce de Dieu démontrée à la croix du Seigneur
            Jésus Christ.
        </p>
        <p>
            Notre but ? Être sel et lumière dans un monde qui a besoin de Dieu.
        </p>
        <p>
            Notre vision ? Être des disciples de Jésus-Christ qui en forment
            d'autres.
        </p>
        <p>
            Soyez les bienvenus chez nous ! Nous anticipons avec joie votre
            prochaine visite.
        </p>
        <p>Nous sommes une communauté de Chrétiens Protestants Évangéliques.</p>
        <p>
            Notre identité ? C'est celle d'individus pécheurs pardonnés et
            renouvelés par la grâce de Dieu démontrée à la croix du Seigneur
            Jésus Christ.
        </p>
        <p>
            Notre but ? Être sel et lumière dans un monde qui a besoin de Dieu.
        </p>
        <p>
            Notre vision ? Être des disciples de Jésus-Christ qui en forment
            d'autres.
        </p>
        <p>
            Soyez les bienvenus chez nous ! Nous anticipons avec joie votre
            prochaine visite.
        </p>
        <p>Nous sommes une communauté de Chrétiens Protestants Évangéliques.</p>
        <p>
            Notre identité ? C'est celle d'individus pécheurs pardonnés et
            renouvelés par la grâce de Dieu démontrée à la croix du Seigneur
            Jésus Christ.
        </p>
        <p>
            Notre but ? Être sel et lumière dans un monde qui a besoin de Dieu.
        </p>
        <p>
            Notre vision ? Être des disciples de Jésus-Christ qui en forment
            d'autres.
        </p>
        <p>
            Soyez les bienvenus chez nous ! Nous anticipons avec joie votre
            prochaine visite.
        </p> -->
</div>

<!-- {#snippet mySnippet(number : number)}
    <h2>Coucou {number}</h2>
{/snippet} -->
