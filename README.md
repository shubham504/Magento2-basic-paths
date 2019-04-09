# Magento2-basic-paths

magento fevicon:= C:\xampp\htdocs\magentot\update\pub
magento head:= C:\xampp\htdocs\magentot\app\design\frontend\Sm\emarket\Magento_Theme\layout
magento css:= C:\xampp\htdocs\magentot\pub\static\frontend\Sm\emarket\en_US\css


this is the basic path of magento-2



# Call Blocks 
```
# .phtml 

<?php echo $this->getLayout() ->createBlock('Magento\Cms\Block\Block') ->setBlockId('your_block_identifier') ->toHtml(); ?>


# CMS Static Block

{{block class="Magento\\Cms\\Block\\Block" block_id="block_identifier"}}

# .xml

<referenceContainer name="content"> 
    <block class="Magento\Cms\Block\Block" name="block_identifier"> 
        <arguments> 
            <argument name="block_id" xsi:type="string">block_identifier</argument> 
        </arguments> 
    </block> 
</referenceContainer>
```
