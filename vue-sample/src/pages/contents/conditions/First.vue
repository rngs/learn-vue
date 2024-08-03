<template>
    <div>
        <Subtitle label="サブタイトル"/>

        <SingleColumn
            id="item1"
            value="value1"
            label="項目①"
        >
            <TextForm id="item1" value="value1" />
        </SingleColumn>

        <DoubleColumn
            :properties="doubles"
        >
            <template v-for="double in doubles" v-slot:[double.id]>
                <TextForm :id="double.id" :value="double.value" :key="double.key"/>
            </template>
        </DoubleColumn>

        <TripleColumn
            :properties="triples"
        >
            <template v-for="triple in triples" v-slot:[triple.id]>
                <TextForm :id="triple.id" :value="triple.value" :key="triple.key"/>
            </template>
        </TripleColumn>
    </div>
</template>

<script>
    import TextForm from "../../common/parts/inputs/types/TextForm";
import DoubleColumn from "../../common/snipets/inputs/layouts/DoubleColumn";
import SingleColumn from "../../common/snipets/inputs/layouts/SingleColumn";
import TripleColumn from "../../common/snipets/inputs/layouts/TripleColumn";
import Subtitle from "../../common/snipets/titles/Subtitle";

import { informations } from "../../scripts/data/informations";

    const doubles = [
        Object.assign(informations.double1, { label: "項目②" }),
        Object.assign(informations.double2, { label: "項目③" })
    ];

    const triples = [
        Object.assign(informations.triple1, { label: "項目④" }),
        Object.assign(informations.triple2, { label: "項目⑤" }),
        Object.assign(informations.triple3, { label: "項目⑥" })
    ];

    export default {
        components: {
            DoubleColumn,
            SingleColumn,
            Subtitle,
            TextForm,
            TripleColumn
        },
        data() {
            return {
                doubles,
                triples
            };
        }
    };
</script>
