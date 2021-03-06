<template>
    <section class="section section-ui-tabs">
        <h2 class="section-heading">UiTabs &amp; UiTab</h2>

        <p>The UiTabs and UiTab components are used together to create a tab container with one or more tabs. Only a UiTab component should be a direct child of UiTabs.</p>

        <p>UiTabs is the tab container and it's props is what you use to customize the tab headers. UiTab is a single tab on which you set tab-specific props including <code>id</code>, <code>header</code>, <code>icon</code> and <code>disabled</code>.</p>

        <p>UiTabs can be one of three types: <code>text</code> (for text only), <code>icon</code> (for icon only) or <code>icon-and-text</code>. The tab headers can also be fullwidth or take up only as much space as needed. The tab container can also be raised to add a drop shadow.</p>

        <p>UiTabs header can be any of four possible background colors: <code>default</code>, <code>primary</code>, <code>accent</code> and <code>clear</code>. The header text color, header active text color and the active tab indicator colors can also be customized.</p>

        <h3>Examples</h3>

        <div class="demo">
            <h4>Text only</h4>

            <ui-tabs type="text">
                <ui-tab header="Books">
                    My books

                    <a href="gogole.com">Hey</a>
                </ui-tab>

                <ui-tab header="Authors">
                    Authors
                </ui-tab>

                <ui-tab header="Collections">
                    My collections
                </ui-tab>

                <ui-tab header="Favourites">
                    My favourites
                </ui-tab>
            </ui-tabs>

            <h4>Text only, fullwidth</h4>

            <ui-tabs fullwidth>
                <ui-tab header="Books">
                    My books
                </ui-tab>

                <ui-tab header="Authors">
                    Authors
                </ui-tab>

                <ui-tab header="Collections">
                    My collections
                </ui-tab>

                <ui-tab header="Favourites">
                    My favourites
                </ui-tab>
            </ui-tabs>

           <h4>Icon only</h4>

            <ui-tabs type="icon">
                <ui-tab icon="book">
                    My books
                </ui-tab>

                <ui-tab icon="person">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Icon only, fullwidth</h4>

            <ui-tabs type="icon" fullwidth>
                <ui-tab icon="book">
                    My books
                </ui-tab>

                <ui-tab icon="person">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Icon and Text</h4>

            <ui-tabs type="icon-and-text">
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Icon and Text, fullwidth</h4>

            <ui-tabs type="icon-and-text" fullwidth>
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Raised</h4>

            <ui-tabs type="icon-and-text" fullwidth raised>
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Background primary</h4>

            <ui-tabs
                type="icon-and-text" fullwidth background-color="primary" text-color="white"
                text-color-active="white" indicator-color="white"
            >
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Background accent</h4>

            <ui-tabs
                type="icon-and-text" fullwidth background-color="accent" text-color="white"
                text-color-active="white" indicator-color="white"
            >
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors">
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>

            <h4>Disabled tab</h4>

            <ui-tabs type="icon-and-text" fullwidth raised>
                <ui-tab icon="book" header="Books">
                    My books
                </ui-tab>

                <ui-tab icon="person" header="Authors" disabled>
                    Authors
                </ui-tab>

                <ui-tab icon="collections_bookmark" header="Collections">
                    My collections
                </ui-tab>

                <ui-tab icon="favorite" header="Favourites">
                    <b>Favourite with longer content</b>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae dolorum laudantium nulla ex asperiores, deserunt quidem perspiciatis eligendi, dolores repudiandae.</p>

                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perferendis hic, aspernatur placeat eligendi delectus laudantium omnis nam consequatur aperiam numquam!</p>
                </ui-tab>
            </ui-tabs>
        </div>

        <h3>API: UiTabs</h3>

        <ui-tabs raised>

            <ui-tab header="Props">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Type</th>
                            <th>Default</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td>type</td>
                                <td>String</td>
                                <td><code>"text"</code></td>
                                <td>The type of tabs. One of <code>text</code>, <code>icon</code> or <code>icon-and-text</code>.</td>
                            </tr>

                            <tr>
                                <td>activeTab</td>
                                <td>String</td>
                                <td class="no-wrap">(The first tab in the set)</td>
                                <td>The <code>id</code> of the tab to select initially.</td>
                            </tr>

                            <tr>
                                <td>backgroundColor</td>
                                <td>String</td>
                                <td><code>"default"</code></td>
                                <td>The background color of the tab headers. One of <code>default</code>, <code>primary</code>, <code>accent</code> or <code>clear</code>.</td>
                            </tr>

                            <tr>
                                <td>textColor</td>
                                <td>String</td>
                                <td><code>"black"</code></td>
                                <td>The text and icon color of the deselected tab headers. One of <code>black</code> or <code>white</code>.</td>
                            </tr>

                            <tr>
                                <td>textColorActive</td>
                                <td>String</td>
                                <td><code>"primary"</code></td>
                                <td>The text and icon color of the selected tab header. One of <code>primary</code>, <code>accent</code> or <code>white</code>.</td>
                            </tr>

                            <tr>
                                <td>indicatorColor</td>
                                <td>String</td>
                                <td><code>"primary"</code></td>
                                <td>The color of the selected tab indicator. One of <code>primary</code>, <code>accent</code> or <code>white</code>.</td>
                            </tr>

                            <tr>
                                <td>fullwidth</td>
                                <td>Boolean</td>
                                <td><code>false</code></td>
                                <td>Determines whether or not the tab header items expand to fill the space available. Set to <code>true</code> for a fullwidth tab header.</td>
                            </tr>

                            <tr>
                                <td>raised</td>
                                <td>Boolean</td>
                                <td><code>false</code></td>
                                <td>Determines whether or not the tab container has a drop shadow. Set to <code>true</code> to raise the tabs.</td>
                            </tr>

                            <tr>
                                <td>hideRippleInk</td>
                                <td>Boolean</td>
                                <td><code>false</code></td>
                                <td>Determines whether or not the ripple ink animation is hidden when a tab header is clicked. Set to <code>true</code> to hide the ripple ink animation.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

            <ui-tab header="Slots">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td>(default)</td>
                                <td>The default slot holds the child UiTab components.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

            <ui-tab header="Events">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Type</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td class="no-wrap">active-tab-changed</td>
                                <td>Dispatched</td>
                                <td>Dispatched when the active tab is changed. Listen for it using <code>@active-tab-changed</code>.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

        </ui-tabs>

        <h3>API: UiTab</h3>

        <ui-tabs raised>

            <ui-tab header="Props">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Type</th>
                            <th>Default</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td>id</td>
                                <td>String</td>
                                <td class="no-wrap">(Auto-generated unique ID)</td>
                                <td>The tab id. Will be applied as <code>id</code> attribute on the tab and used when setting a default tab.</td>
                            </tr>

                            <tr>
                                <td>header</td>
                                <td>String</td>
                                <td></td>
                                <td>The tab header (text only).</td>
                            </tr>

                            <tr>
                                <td>icon</td>
                                <td>String</td>
                                <td></td>
                                <td>The tab icon. Can be any of the <a href="https://design.google.com/icons/" target="_blank">Material Icons</a>. Note that this should be the icon codepoint if you want to support IE9.</td>
                            </tr>

                            <tr>
                                <td>disabled</td>
                                <td>Boolean</td>
                                <td><code>false</code></td>
                                <td>Determines whether or not the tab can be selected. Set to <code>true</code> to disable the tab and prevent user interactions.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

            <ui-tab header="Slots">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td>(default)</td>
                                <td>The default slot holds the tab content and can contain HTML.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

            <ui-tab header="Events">
                <div class="table-responsive">

                    <table class="table">
                        <thead>
                            <th>Name</th>
                            <th>Type</th>
                            <th>Description</th>
                        </thead>

                        <tbody>
                            <tr>
                                <td class="no-wrap">selected</td>
                                <td>Dispatched</td>
                                <td>Dispatched when the tab is selected. The handler is called with the tab's <code>id</code>. Listen for it using <code>@selected</code>.</td>
                            </tr>

                            <tr>
                                <td class="no-wrap">deselected</td>
                                <td>Dispatched</td>
                                <td>Dispatched when the tab is deselected (i.e. when the user selects another tab). The handler is called with the tab's <code>id</code>. Listen for it using <code>@deselected</code>.</td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </ui-tab>

        </ui-tabs>

    </section>
</template>

<script>
import UiTab from '../../src/UiTab.vue';
import UiTabs from '../../src/UiTabs.vue';

export default {
    components: {
        UiTab,
        UiTabs
    }
};
</script>

<style lang="stylus">
.section-ui-tabs {
    //
}
</style>
