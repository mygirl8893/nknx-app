<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!"/>
        <TabView android:tabBackgroundColor="#53ba82" android:tabTextColor="#c4ffdf" android:selectedTabTextColor="#ffffff" androidSelectedTabHighlightColor="#ffffff" androidTabsPosition="bottom">
            <TabViewItem title="Tab 1">
                <GridLayout columns="*" rows="*">
                    <NodesManager></NodesManager>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="Tab 2">
                <GridLayout columns="*" rows="*">
                    <WalletTracker></WalletTracker>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="Tab 3">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Tab 3 Content" col="0" row="0" />
                </GridLayout>
            </TabViewItem>
        </TabView>
    </Page>
</template>

<script>
import NodesManager from './NodesManager';
import WalletTracker from './WalletTracker';

export default {
	components: {
		NodesManager,
		WalletTracker
	},
    data() {
        return {
            msg: 'Hello World!'
        }
    }
}
</script>