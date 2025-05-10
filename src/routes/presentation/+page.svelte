<script lang="ts">
    import type { PageData } from "./$types";

    let { data }: { data: PageData } = $props();
</script>

<div class="relative h-96 w-full mb-10 flex items-start">
    <div
        class="absolute top-0 left-0 h-full w-full bg-[url('/BG-presentation.png')] bg-cover bg-center -z-10"
    >
        <div class="flex flex-col ml-[25vw] mt-32">
            <h1 class="relative text-white text-4xl">Qui sommes-nous ?</h1>
        </div>
    </div>
</div>
<div class="ml-60 mr-60 mb-25">
    <h2 class="text-3xl pb-5 pt-5">Nous sommes Chrétiens</h2>
    <p>
        Nous nous attachons à l’enseignement de Jésus-Christ. Nous comprenons
        qu’il est Dieu, venu « en chair et en os » afin de révéler pleinement la
        divinité et d’indiquer le chemin qui mène à Lui.
    </p>

    <h2 class="text-3xl pb-5 pt-5">Nous sommes Protestants</h2>
    <p>
        Nous nous réclamons de la Réforme du XVIe siècle qui a replacé la Bible
        au centre de la vie chrétienne. Nous cherchons à conformer notre vie et
        notre enseignement à la Bible. C’est de cette dernière que nous tirons
        notre foi et nos pratiques et en priorité sur les traditions et les
        expériences humaines.
    </p>

    <h2 class="text-3xl pb-5 pt-5">Nous sommes Évangéliques</h2>
    <p>
        Nous croyons qu’il faut volontairement et personnellement devenir
        chrétien. Nul ne naît chrétien. On le devient par une décision
        personnelle. Nous ne pratiquons donc pas le baptême des enfants, car
        nous estimons que ce choix leur incombe. Notre église appartient ainsi
        aux assemblées dites « de confessants » c’est-à-dire d’individus devenus
        chrétiens par choix.<br /> Nous croyons à l’autonomie des églises
        locales. Aucune hiérarchie nationale ou internationale ne peut imposer
        sa doctrine ou ses pratiques à l’église locale. Ceci explique la
        diversité des noms (et des qualités!) de la mouvance évangélique.<br /> Nous
        nous situons dans l’aile plutôt conservatrice du mouvement évangélique.
    </p>
</div>
