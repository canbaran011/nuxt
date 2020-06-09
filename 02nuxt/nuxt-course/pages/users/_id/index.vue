<template>
    <div>
        <h2>
            A single user page with ID : {{ $route.params.id }}
        </h2>
        
    </div>
</template>
<script>
export default {
    validate(data){
        console.log(data)
        return /^\d+$/.test(data.params.id)
    },
    layout : 'users'
}
</script>