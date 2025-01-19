<script>
    import "../app.css";
    import Header from "../components/Header.svelte";
    import ContactUs from "../components/ContactUs.svelte";
</script>

<div>
    <Header />
    <slot />
    <ContactUs />
</div>
