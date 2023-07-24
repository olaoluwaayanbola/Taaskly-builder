<template>
    <div class="container">
        <div class="block_one">
            <span class="title"></span>
            <span class="close"></span>
        </div>
        <div class="formv">
            <form action="" class="form1">
                <section>
                    <h2>Details</h2>
                    <div class="bill_from_to">
                        <label for="billFrom">Bill from</label>
                        <input type="text" id="billFrom" v-model="billFrom" />

                        <label for="billTo">Bill to</label>
                        <input type="text" id="billTo" v-model="billTo" />
                    </div>

                    <label for="recipientEmail">Recipient Email</label>
                    <input type="email" id="recipientEmail" v-model="recipientEmail" />

                    <label for="billTitle">Bill Title/Project Description</label>
                    <input type="text" id="billTitle" v-model="billTitle" />

                    <div class="issued_on_due_on">
                        <label for="issuedOn">Issued on</label>
                        <input type="date" id="issuedOn" v-model="issuedOn" />

                        <label for="dueOn">Due on</label>
                        <input type="date" id="dueOn" v-model="dueOn" />
                    </div>

                    <input type="checkbox" name="sendCopy" id="sendCopy" v-model="sendCopy" />
                </section>

                <section>
                    <h2>Invoice Item</h2>

                    <label for="">currency</label>
                    <input type="text" id="currency" v-model="currency" />
                    <span id="dropdown_logo">^</span>

                    <div class="item-row">
                        <label for="">Item</label>
                        <input type="text" />

                        <label for="">Price</label>
                        <input type="text" />

                        <label for="">Quantity</label>
                        <input type="text" />

                        <label for="">Total Price</label>
                        <input type="text" disabled />
                    </div>

                    <div class="add_total">
                        <span><i class="logo"></i>Add item</span>
                        <span>Total Amount</span>
                        <span>$500</span>
                    </div>
                </section>

                <section>
                    <label for="notes"></label>
                    <textarea name="notes" id="notes" cols="30" rows="10"></textarea>
                </section>
                <button>Create invoice</button>
            </form>
        </div>
    </div>
</template>
<script>
export default {

}
</script>

<style>
.container {
    background-color: whitesmoke;
}
</style>