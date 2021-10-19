<template>
  <nav>
    <ul class="list-disc ">
      <li>
        <NavLink href="/" :active="$page.component === 'Home'">
          Home
        </NavLink>
      </li>

      <li>
        <NavLink href="/users" :active="$page.component === 'Users'">
          Users
        </NavLink>
      </li>

      <li>
        <NavLink href="/settings" :active="$page.component === 'Settings'">
          Settings
        </NavLink>
      </li>

      <li>
        <NavLinkLogout href="/logout">
          Log out
        </NavLinkLogout>
      </li>

    </ul>
  </nav>
</template>

<script>
import NavLink from "./NavLink";
import NavLinkLogout from "./NavLinkLogout";
export default {
  components: { NavLink, NavLinkLogout },
};
</script>