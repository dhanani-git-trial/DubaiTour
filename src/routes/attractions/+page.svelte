<script>
    import AttractionCard from "$components/AttractionCard.svelte";
    import A from "$components/pins/A.svelte";
    import B from "$components/pins/B.svelte";
    import C from "$components/pins/C.svelte";
    import D from "$components/pins/D.svelte";
    import E from "$components/pins/E.svelte";
    import F from "$components/pins/F.svelte";
    import G from "$components/pins/G.svelte";
    import H from "$components/pins/H.svelte";
    import I from "$components/pins/I.svelte";
    import Nav from "$components/Nav.svelte";
</script>
<Nav/>
<br /><br /><br />
<div class="cards-container">
    <!--HERE ↓-->
    <div class="box">
        <AttractionCard
            ><span slot="title"><A />The Burj Khalifa</span><span
                slot="subtitle"
                >The Burj Khalifa is regarded as the World's Tallest Building:
                At a staggering height of 828 meters (2,717 feet), the Burj
                Khalifa is the tallest building in the world. Tourists can visit
                the "At the Top" observation deck on the 148th floor for
                stunning views of the city and the desert. The Burj Khalifa also
                hosts some of Dubai's finest restaurants and a high-end lounge.</span
            >
            
            </AttractionCard
        >
        <img width="320" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c5/Dubai_Skyline_with_Ra%27s_Al_Khor_Wildlife_Sanctuary.jpg/1280px-Dubai_Skyline_with_Ra%27s_Al_Khor_Wildlife_Sanctuary.jpg" alt=""/>
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><B />The Dubai Mall</span><span slot="subtitle"
                >The Dubai Mall is a Massive Shopping Center: One of the largest
                shopping malls in the world, it features over 1,200 shops, a
                giant aquarium, an indoor ice rink, and even a VR park. The
                Dubai Aquarium & Underwater Zoo Is home to thousands of aquatic
                animals, it's one of the largest suspended aquariums in the
                world.</span
            ></AttractionCard
        >
        <img width="320" alt="" src="https://upload.wikimedia.org/wikipedia/commons/d/df/Dubai_Mall_10.jpg">
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title">Dubai's Food Scene</span><span slot="subtitle"
                >Dubai is a melting pot of cultures, and its food scene reflects
                that. From street food to Michelin-starred restaurants, visitors
                can indulge in global flavors—try Emirati dishes like Al Harees,
                Shawarma, or a delicious Arabic breakfast. Brunch Culture in
                Dubai is famous for its lavish Friday brunches, where luxury
                hotels offer gourmet buffets and live entertainment.</span
            >
        </AttractionCard>
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><C />The Dubai Fountain</span><span
                slot="subtitle"
                >The Dubai Fountain is renowned for its Impressive Water Shows:
                Set at the base of the Burj Khalifa, the Dubai Fountain features
                nightly water shows set to music and lights. The fountains shoot
                water 500 feet into the air, synchronized with a variety of
                music.</span
            ></AttractionCard
        >
        <img width="320" src="https://lh5.googleusercontent.com/p/AF1QipMC5x5erWlAHMyyGUN_T12rX2HDXCxB6Q4Aj1Ls=w270-h312-n-k-no">
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><D />The Palm Jumeirah</span><span
                slot="subtitle"
                >The Palm Jumeirah is one of the world's most famous man-made
                islands, shaped like a palm tree. It's home to luxury hotels,
                including the famous Atlantis The Palm, which boasts the
                Aquaventure Waterpark.</span
            ></AttractionCard
        >
        <img width="320" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/15/Artificial_Archipelagos%2C_Dubai%2C_United_Arab_Emirates_ISS022-E-024940_lrg.jpg/1280px-Artificial_Archipelagos%2C_Dubai%2C_United_Arab_Emirates_ISS022-E-024940_lrg.jpg" alt=""/>
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title">Desert Safari</span><span slot="subtitle"
                >You can also go on a Desert Safari in Dubai, a thrilling desert
                adventure where tourists can experience dune bashing, camel
                rides, and traditional Bedouin-style camps with food,
                entertainment, and stargazing in the Arabian Desert.</span
            ></AttractionCard
        >
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><E />The Jumeirah Beach</span><span
                slot="subtitle"
                >The Jumeirah Beach is an Iconic Beach Destination: The Jumeirah
                Beach offers stunning views of the Burj Al Arab, one of the most
                photographed hotels in the world. The beach is perfect for
                sunbathing, swimming, and water sports.</span
            ></AttractionCard
        >
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><F />Expo City Dubai</span><span slot="subtitle"
                >Expo City Dubai was originally the site of the World Expo 2020,
                Expo City Dubai now hosts permanent and temporary exhibitions,
                offering a peek into the future of technology, sustainability,
                and global collaboration.</span
            ></AttractionCard
        >
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><G />The Dubai World Cup</span><span
                slot="subtitle"
                >The Dubai World Cup is Horse Racing’s Biggest Event: If you're
                in Dubai in March, the Dubai World Cup is one of the richest
                horse races in the world, held at the Meydan Racecourse.</span
            ></AttractionCard
        >
    </div>
    <div class="box">
        <AttractionCard
            ><span slot="title"><H />Dubai Creek</span><span slot="subtitle"
                >Dubai Creek & Old Dubai carries a significant amount of
                historical charm, Dubai’s roots lie in the Creek area. Visitors
                can take an abra (traditional wooden boat) ride along the water
                and explore the Gold Souk (market) and Spice Souk for a taste of
                Dubai’s trading history.</span
            ></AttractionCard
        >
        <img width="320" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/76/The_view_of_Dubai_Creek.jpg/1280px-The_view_of_Dubai_Creek.jpg" alt=""/>
    </div>
    
    <div class="box">
        <AttractionCard
            ><span slot="title"><I />Dubai's Miracle Garden</span><span
                slot="subtitle"
                >The only way to describe Dubai’s Miracle Garden is nothing less
                than a Floral Wonderland: The Dubai Miracle Garden is the
                world’s largest natural flower garden, featuring over 45 million
                flowers. It's a stunning display of vibrant colors and floral
                sculptures, open during the cooler months.</span
            ></AttractionCard
        >
    </div>
</div>

<style>
    .cards-container {
        display: grid;
        grid-template-columns: repeat(3, 1fr); /* 3 columns, equally spaced */
        gap: 20px; /* Adjust the space between cards */
        grid-row-gap: 30px;
        padding: 20px;
        font-family: "Kanit";
    }

    span {
        display: flex;
    }

    img {
        border-radius: 20px;
        height: auto !important;
        filter: none !important;
    }
</style>
