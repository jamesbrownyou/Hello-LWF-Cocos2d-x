Hello-LWF-Cocos2d-x
===================

Notice
-------------------

This project does not use any texture atlas and batch node. It means that this project is not intended to show the rendering performance using LWF on cocos2d-x.

How to use LWFNode with SpriteBatchNode
-------------------

    LWFNode *lwfNode = LWFNode::create("sample.lwf");
    SpriteBatchNode *batch = SpriteBatchNode::createWithTexture(lwfNode->getTexture());
    batch->addChild(lwfNode);
    this->addChild(batch);

sample.lwf should be converted with one texture atlas.

