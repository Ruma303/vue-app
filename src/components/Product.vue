    <script setup>
    const props = defineProps({
        componentTitle: {
            type: String,
            required: true
        },
        componentDescription: {
            type: String,
            required: true
        },
        price: {
            type: Number,
            required: true
        },
        quantity: {
            type: Number,
            default: 0,
        }
    });
    const methods = {
        buy() {
            this.$emit('buy-product');
        }
    }
    </script>

    <template>
        <h1>{{ componentTitle }}</h1>
        <p>{{ componentDescription }}</p>
        <p>{{ price }}€</p>
        <button @click="$emit('buy', 1)">Buy</button>
    </template>

