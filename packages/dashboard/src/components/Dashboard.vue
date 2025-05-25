<template>
  <div class="dashboard">
    <!-- Sidebar -->
    <aside class="sidebar">
      <h2 class="logo">My Dashboard</h2>
      <nav>
        <ul>
          <li><a href="#">Overview</a></li>
          <li><a href="#">Reports</a></li>
          <li><a href="#">Settings</a></li>
        </ul>
      </nav>
    </aside>

    <!-- Main Content -->
    <div class="main">
      <header class="topbar">
        <h1>Dashboard</h1>
      </header>

      <section class="content">
        <div class="card">Card 1</div>
        <div class="card">Card 2</div>
        <div class="card">Card 3</div>
      </section>
    </div>
  </div>
</template>

<script setup>
// No JS logic for now, it's a static layout
</script>

<style scoped>
.dashboard {
  display: flex;
  height: 100vh;
  font-family: Arial, sans-serif;
}

.sidebar {
  width: 220px;
  background-color: #2c3e50;
  color: #ecf0f1;
  padding: 20px;
}

.sidebar .logo {
  margin-bottom: 20px;
  font-size: 1.5em;
}

.sidebar ul {
  list-style: none;
  padding: 0;
}

.sidebar ul li a {
  color: #ecf0f1;
  text-decoration: none;
  display: block;
  margin: 10px 0;
}

.sidebar ul li a:hover {
  text-decoration: underline;
}

.main {
  flex-grow: 1;
  background-color: #f4f6f8;
  display: flex;
  flex-direction: column;
}

.topbar {
  background-color: #fff;
  padding: 16px 24px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.content {
  flex-grow: 1;
  padding: 24px;
  display: flex;
  gap: 16px;
}

.card {
  flex: 1;
  background: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}
</style>
