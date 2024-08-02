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
            id="item1"
            value="value1"
            label="項目①"
        >
            <TextForm id="item1" value="value1" />
        </DoubleColumn>

        <TripleColumn
            id="item1"
            value="value1"
            label="項目①"
        >
            <TextForm id="item1" value="value1" />
        </TripleColumn>
<!-- 
        <b-container class="text-start text-nowrap mb-2">
            <b-row>
                <b-col sm="6">
                    <FormGroup
                        id="item2"
                        value="value2"
                        label="項目②"
                        label-cols="4"
                        content-cols="8"
                    >
                        <TextForm id="item2" value="value2" />
                    </FormGroup>
                </b-col>
                <b-col sm="6">
                    <FormGroup
                        id="item3"
                        value="value3"
                        label="項目③"
                        label-cols="4"
                        content-cols="8"
                    >
                        <TextForm id="item3" value="value3" />
                    </FormGroup>
                </b-col>
            </b-row>
        </b-container>

        <b-container class="text-start text-nowrap mb-2">
            <b-row>
                <b-col sm="4">
                    <FormGroup
                        id="item4"
                        value="value4"
                        label="項目④"
                        label-cols="6"
                        content-cols="6"
                    >
                        <TextForm id="item4" value="value4" />
                    </FormGroup>
                </b-col>
                <b-col sm="4">
                    <FormGroup
                        id="item5"
                        value="value5"
                        label="項目⑤"
                        label-cols="6"
                        content-cols="6"
                    >
                        <TextForm id="item5" value="value5" />
                    </FormGroup>
                </b-col>
                <b-col sm="4">
                    <FormGroup
                        id="item6"
                        value="value6"
                        label="項目⑥"
                        label-cols="6"
                        content-cols="6"
                    >
                        <TextForm id="item6" value="value6" />
                    </FormGroup>
                </b-col>
            </b-row>
        </b-container>
-->
    </div>
</template>

<script>
    import TextForm from "../../common/parts/inputs/types/TextForm";
// import FormGroup from "../../common/snipets/inputs/FormGroup";
import DoubleColumn from "../../common/snipets/inputs/layouts/DoubleColumn";
import SingleColumn from "../../common/snipets/inputs/layouts/SingleColumn";
import TripleColumn from "../../common/snipets/inputs/layouts/TripleColumn";
import Subtitle from "../../common/snipets/titles/Subtitle";

    export default {
        components: {
            DoubleColumn,
            // FormGroup,
            SingleColumn,
            Subtitle,
            TextForm,
            TripleColumn
        }
    };
</script>
