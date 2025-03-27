<script>
    // Import global CSS if needed
</script>

<div class="app">
    <header>
        <div class="header-content">
            <h1>SYNTAXSPHERE - AI</h1>
            <nav>
                <a href="/">Home</a>
                <a href="/dashboard">Dashboard</a>
                <a href="/integrations">Integrations</a>
            </nav>
        </div>
    </header>

    <main>
        <slot />
    </main>

    <footer>
        <p>© 2025 SYNTAXSPHERE - AI | The Command Center for Small Business Ops</p>
    </footer>
</div>

<style>
    .app {
        display: flex;
        flex-direction: column;
        min-height: 100vh;
    }

    header {
        background: linear-gradient(to right, #1a1a2e, #16213e);
        color: white;
        padding: 1rem;
    }

    .header-content {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    nav a {
        color: white;
        margin-left: 1.5rem;
        text-decoration: none;
    }

    nav a:hover {
        text-decoration: underline;
    }

    main {
        flex: 1;
        padding: 2rem;
        max-width: 1200px;
        margin: 0 auto;
        width: 100%;
    }

    footer {
        background: #1a1a2e;
        color: white;
        padding: 1rem;
        text-align: center;
    }
</style>