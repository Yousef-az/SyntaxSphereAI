<script>
    import { goto } from '$app/navigation';

    function navigateToDashboard() {
        goto('/dashboard');
    }
</script>

<section class="hero">
    <h1>SYNTAXSPHERE - AI</h1>
    <h2>The All-in-One Command Center for Small Business Operations</h2>
    <p>Connect, automate, and manage all your existing tools — Slack, Zoho, Salesforce, Gmail, Stripe — from one unified interface.</p>
    <button on:click={navigateToDashboard}>Launch Command Center</button>
</section>

<section class="features">
    <div class="feature-card">
        <h3>Platform Integrations</h3>
        <p>Connect all your business tools with seamless OAuth integrations</p>
    </div>

    <div class="feature-card">
        <h3>AI-Powered Automations</h3>
        <p>Intelligent workflows that learn and adapt to your business needs</p>
    </div>

    <div class="feature-card">
        <h3>Smart Command Center</h3>
        <p>Monitor all incoming messages, tasks, and sales activity in one place</p>
    </div>
</section>

<style>
    .hero {
        text-align: center;
        padding: 4rem 1rem;
        background: linear-gradient(135deg, #f5f7fa 0%, #e4e7eb 100%);
        border-radius: 12px;
        margin-bottom: 2rem;
    }

    h1 {
        font-size: 3.5rem;
        margin-bottom: 0.5rem;
        background: linear-gradient(to right, #1a1a2e, #16213e);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    h2 {
        font-size: 1.5rem;
        color: #16213e;
        margin-bottom: 1.5rem;
    }

    p {
        max-width: 800px;
        margin: 0 auto 2rem;
        font-size: 1.2rem;
        line-height: 1.6;
        color: #4a4a4a;
    }

    button {
        background: linear-gradient(to right, #0070f3, #1a1a2e);
        color: white;
        border: none;
        padding: 0.75rem 1.75rem;
        border-radius: 4px;
        font-size: 1.1rem;
        font-weight: 600;
        cursor: pointer;
        transition: transform 0.2s;
    }

    button:hover {
        transform: translateY(-2px);
    }

    .features {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
        margin-top: 3rem;
    }

    .feature-card {
        background: white;
        padding: 2rem;
        border-radius: 8px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        transition: transform 0.3s;
    }

    .feature-card:hover {
        transform: translateY(-5px);
    }

    .feature-card h3 {
        margin-top: 0;
        color: #16213e;
    }
</style>