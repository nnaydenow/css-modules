<script>
	import "@ui5/webcomponents/dist/Icon";
	import "@ui5/webcomponents/dist/Title";
	import "@ui5/webcomponents/dist/Input";
	import "@ui5/webcomponents/dist/Link";



	import "@ui5/webcomponents-fiori/dist/ShellBar";
	import "@ui5/webcomponents-fiori/dist/SideNavigation";
	import "@ui5/webcomponents-fiori/dist/SideNavigationItem";
	import "@ui5/webcomponents-fiori/dist/SideNavigationSubItem";
	import "@ui5/webcomponents-icons/dist/person-placeholder"

	import "@ui5/webcomponents-icons/dist/search";
	import "@ui5/webcomponents-icons/dist/home";
	import "@ui5/webcomponents-icons/dist/play";
	import "@ui5/webcomponents-icons/dist/slim-arrow-right";

	import toolLayoutStyles from "@ui5/webcomponents-fiori/dist/styles/ToolLayout.module.css"
	import linkStyles from "@ui5/webcomponents/dist/styles/Link.module.css"
	import inputStyles from "@ui5/webcomponents/dist/styles/Input.module.css"
</script>

   <div class={toolLayoutStyles.toolLayout}>
      <ui5-shellbar
        class={toolLayoutStyles.shellBar}
        primary-title="Product Name"
        secondary-title="Second Title"
        notifications-count="1"
        show-notifications>
        <ui5-input slot="searchField"></ui5-input>
        <ui5-button icon="menu" slot="startButton" id="toggle"></ui5-button>
        <ui5-avatar slot="profile">
          <ui5-icon name="person-placeholder" />
        </ui5-avatar>
      </ui5-shellbar>

      <ui5-side-navigation class={toolLayoutStyles.sideNavigation}>
        <ui5-side-navigation-item text="Home" icon="home"></ui5-side-navigation-item>
        <ui5-side-navigation-item text="People" expanded icon="group">
          <ui5-side-navigation-sub-item text="From My Team"></ui5-side-navigation-sub-item>
          <ui5-side-navigation-sub-item text="From Other Team"></ui5-side-navigation-sub-item>
        </ui5-side-navigation-item>
        <ui5-side-navigation-item text="Locations" icon="locate-me" selected></ui5-side-navigation-item>
        <ui5-side-navigation-item text="Events" icon="calendar">
          <ui5-side-navigation-sub-item text="Local"></ui5-side-navigation-sub-item>
          <ui5-side-navigation-sub-item text="Others"></ui5-side-navigation-sub-item>
        </ui5-side-navigation-item>
        <ui5-side-navigation-item slot="fixedItems" text="Useful Links" icon="chain-link"></ui5-side-navigation-item>
        <ui5-side-navigation-item slot="fixedItems" text="History" icon="history"></ui5-side-navigation-item>
      </ui5-side-navigation>
      <div class={toolLayoutStyles.content}>
        <ui5-title level="H3">Input</ui5-title>
        <ui5-input>
          <ui5-icon name="search" slot="icon" class={inputStyles.inputIcon}></ui5-icon>
        </ui5-input>
        <ui5-title level="H3">Link</ui5-title>
        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" disabled target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" target="_blank">
          sap.com
          <ui5-icon class={linkStyles.linkIconEnd} name="slim-arrow-right"></ui5-icon>
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" target="_blank">
          <ui5-icon name="play"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" disabled design="Subtle" target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" design="Subtle" target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" disabled design="Emphasized" target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>

        <br />

        <ui5-link class={linkStyles.linkWithIcon} href="https://www.sap.com" design="Emphasized" target="_blank">
          <ui5-icon name="home"></ui5-icon>
          sap.com
        </ui5-link>
      </div>
    </div>