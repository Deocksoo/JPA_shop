<template>
	<div class="newOrder">
		<h1>상품 주문</h1>
		
		<v-flex xs12 sm6 md6 my-auto pt-6>
			<v-autocomplete label="주문 회원" :items="orderMembers" clearable></v-autocomplete>
			<v-autocomplete label="상품명" :items="items" clearable></v-autocomplete>
			<v-text-field label="주문 수량" placeholder="주문 수량을 입력하세요" clearable></v-text-field>
			
			<v-layout justify-end>
				<v-btn fab dark small color="light-green lighten-2" class="mr-2">
					<v-icon>done</v-icon>
				</v-btn>
				<v-btn fab dark small color="red lighten-2">
					<v-icon>clear</v-icon>
				</v-btn>
			</v-layout>
		</v-flex>
	</div>
</template>

<script>
    export default {
        name: "NewOrder",
        data() {
            return {
                orderMembers: [],
                items: []
            }
        }
    }
</script>

<style scoped>

</style>