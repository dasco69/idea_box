<template>
    <div class="grid grid-flow-col grid-cols-2 h-body  flex items-center">
        <div>
            <ACardBasic>
                <template v-slot:title>
                    <ATitle title="Ton Idées" classCss="text-blue-300"/>
                </template>
                <template v-slot:input>
                    <ATextArea label="Écris ce qui te ferais envie." classCss="text-blue-300"/>
                </template>
                <template v-slot:button>
                    <AButtonForm label="Envoyé" classCss="bg-blue-300 transition delay-150 hover:bg-blue-500 focus:outline-none focus:ring-2 focus:ring-purple-600 focus:ring-opacity-50"/>
                </template>
            </ACardBasic>
        </div>
        <div>
            <ACardIdea>
                <template v-slot:title>
                    <ATitle title="Les idées proposés" classCss="text-blue-300"/>
                </template>
                <template v-slot:point>
                    <ASubtitle title="Point de vote restant:" />
                </template>
                <template v-slot:list>
                    <AListIdea />
                </template>
            </ACardIdea>
        </div>
    </div>
</template>

<script>
import AButtonForm from '../components/atoms/button/AButtonForm.vue'
import ACardBasic from '../components/atoms/card/ACardBasic.vue'
import ACardIdea from '../components/atoms/card/ACardIdea.vue'
import ATextArea from '../components/atoms/input/ATextArea.vue'
import AListIdea from '../components/atoms/listIdea/AListIdea.vue'
import ASubtitle from '../components/atoms/title/ASubtitle.vue'
import ATitle from '../components/atoms/title/ATitle.vue'
    export default {
  components: { AButtonForm, ACardBasic, ATitle, ATextArea, ACardIdea, ASubtitle, AListIdea },
        name: 'goodjob',
    }
</script>

<style></style>