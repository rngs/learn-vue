<template>
    <div>
        <Subtitle label="サブタイトル"/>

        <SingleColumn
            id="item1"
            value="value1"
            label="項目①"
        >
            <!-- <TextForm id="item1" value="value1" /> -->
            <!-- <CheckboxForm :id="item1" :value="value1" :options="options" /> -->
             <SelectForm />
        </SingleColumn>

        <DoubleColumn
            :properties="[
                {id: informations.double1.id, label: '項目②'},
                {id: informations.double2.id, label: '項目③'}
            ]"
        >
            <template v-slot:[informations.double1.id]>
                <!-- <TextForm :id="informations.double1.id" :value="informations.double1.value" /> -->
                <SelectForm />
            </template>
            <template v-slot:[informations.double2.id]>
                <CheckboxForm :id="informations.double2.id" :value="informations.double2.value" :options="options" :selected="informations.double2.value" />
            </template>
        </DoubleColumn>

        <TripleColumn
            :properties="[
                {id: informations.triple1.id, label: '項目②'},
                {id: informations.triple2.id, label: '項目③'},
                {id: informations.triple3.id, label: '項目③'}
            ]"
        >
            <template v-slot:[informations.triple1.id]>
                <!-- <TextForm :id="informations.triple1.id" :value="informations.triple1.value" /> -->
                <SelectForm />
            </template>
            <template v-slot:[informations.triple2.id]>
                <TextForm :id="informations.triple2.id" :value="informations.triple2.value" />
            </template>
            <template v-slot:[informations.triple3.id]>
                <TextForm :id="informations.triple3.id" :value="informations.triple3.value" />
            </template>
        </TripleColumn>
    </div>
</template>

<script>
    import CheckboxForm from "../../common/parts/inputs/types/CheckboxForm";
import SelectForm from "../../common/parts/inputs/types/SelectForm";
import TextForm from "../../common/parts/inputs/types/TextForm";
import DoubleColumn from "../../common/snipets/inputs/layouts/DoubleColumn";
import SingleColumn from "../../common/snipets/inputs/layouts/SingleColumn";
import TripleColumn from "../../common/snipets/inputs/layouts/TripleColumn";
import Subtitle from "../../common/snipets/titles/Subtitle";

import { informations } from "../../scripts/data/informations";

    export default {
        components: {
            CheckboxForm,
            DoubleColumn,
            SelectForm,
            SingleColumn,
            Subtitle,
            TextForm,
            TripleColumn
        },
        data() {
            return {
                informations,
                options: [
                    { text: 'First radio', value: 'first' },
                    { text: 'Second radio', value: 'second' },
                    { text: 'Third radio', value: 'double2' }
                ]
            };
        }
    };
</script>
